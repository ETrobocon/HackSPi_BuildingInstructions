# HackSPi submodel structure

## HackSPi_M2


## HackSPi_M2_Arrow
- **HackSPi_M2_FrontChassis_Arrow**
    - **HackSPi_M2_ArmMotor_Arrow**
        - **EpsilonSpikerConcept_LightSensor_Arrow**
        - **HackSPi_M2_BumperSpacer_Arrow**
    - **HackSPi_M2_Apillar_Arrow**
        - **HackSPi_M2_BatterySupport_Arrow**
        - EpsilonSpikerConcept_RasPiSupport
        - **HackSPi_M2_MagentaCableClip_Arrow**
        - **EpsilonSpikerConcept_Roof_Arrow**
    - **HackSPi_M2_FrontChassisJoint_Arrow**
    - **EpsilonSpikerConcept_Head_Arrow**
        - **EpsilonSpikerConcept_Antenna_Arrow**
    - **HackSPi_M2_Wheel_Arrow**
        - **HackSPi_M2_WheelCap_Arrow**
- **HackSPi_M2_RearChassis_Arrow**
    - **EpsilonSpikerConcept_Caster_Arrow**
    - **EpsilonSpikerConcept_RearChassisJoint_Arrow**
- **EpsilonSpikerConcept_RearChassisApillarJoint_Arrow**
- **EpsilonSpikerConcept_Cpillar_GroundCamera_Arrow**
    - **EpsilonSpikerConcept_CameraModule_Arrow**
- **EpsilonSpikerConcept_LeftRearChassisCpillarJoint_Arrow**
- **EpsilonSpikerConcept_RightRearChassisCpillarJoint_Arrow**
- **EpsilonSpikerConcept_LeftApillarCpillarJoint_Arrow**
- **EpsilonSpikerConcept_RightApillarCpillarJoint_Arrow**

## EpsilonSpikerConcept
- EpsilonSpikerConcept_FrontChassis
    - EpsilonSpikerConcept_ArmMotor
        - EpsilonSpikerConcept_LightSensor
    - EpsilonSpikerConcept_Apillar
        - EpsilonSpikerConcept_RasPiSupport
        - EpsilonSpikerConcept_LeftRoof
        - EpsilonSpikerConcept_RightRoof
    - EpsilonSpikerConcept_FrontChassisJoint
    - EpsilonSpikerConcept_Head
        - EpsilonSpikerConcept_Antenna
    - EpsilonSpikerConcept_Wheel
        - EpsilonSpikerConcept_WheelCap
- EpsilonSpikerConcept_RearChassis
    - EpsilonSpikerConcept_Caster
    - EpsilonSpikerConcept_RearChassisJoint
- EpsilonSpikerConcept_RearChassisApillarJoint
- EpsilonSpikerConcept_Cpillar_GroundCamera
    - EpsilonSpikerConcept_CameraModule
- EpsilonSpikerConcept_LeftRearChassisCpillarJoint
- EpsilonSpikerConcept_RightRearChassisCpillarJoint
- EpsilonSpikerConcept_LeftApillarCpillarJoint
- EpsilonSpikerConcept_RightApillarCpillarJoint

# Modeling Tricks
- Settings→Rotation PointからWorld Originを選択して、FrontChassisとRearChassisは、(0,0,0)で接合させる。完成後、最終的にはWorld Originを、ArrowはRearChassisのベースフレーム中央へ、Arrowなしはモータの回転軸（FrontChassisのPartsOrigin）に設定したい。

- FrontChassisの接合点(WorldOrigin)は(0,50,20)なので、PartsOriginをWorldOriginの(0,-50,-20)に置いてからX軸をcosΘ回す。
    - `Y=-SIN(ATAN(50/20)-ACOS(cosΘ))*SQRT(20*20+50*50)`
    - `Z=-COS(ATAN(50/20)-ACOS(cosΘ))*SQRT(20*20+50*50)`
- 接合させるにはcosΘ=0.6回すので、この時のPartsOrigin座標は、(0,-14,-52)となる。
- 一方、ねじって接合させるのに回す角度は45度。これはMLCadのボタン操作でよい。

- RearChassisはEpsilonSpikerではジョイント中央をPartsOriginに設定してしまったが、これを接合面に、cosΘ=0.8立ててからZを-10して修正しておく。この時のベースフレームの中央座標は(0,-9.971,160.037)で、上部を組み立てる際には端数分(0,-0.029,-0.037)移動させて行う。

- Rear Chassis/C Pillarジョイントを打った後で、ここまでの４Ass'yをそれぞれ別々にWorld Originで回す。
    - FrontChassisはボタンで45度回す
    - RearChassisは単位行列に戻す
    - RearChassisCpillarJointもボタンで45度回す。
- RearChassisにあわせて全体を(0,-0.029,-0.037)移動させる
- ねじってRoofとの帳尻をあわせるため、RearChassisのみ(0,19.971,9.963)へ移動させる。


# LPub3D Technics
- LPub3Dは動作が不安定で、元のファイルを頻繁に壊すので、LPubメタコマンドはLPub上で配置してからセーブせずメタコマンドのみをコピーし、VSCode上で編集した方が良い。
- 1:1のモデルでは`0 !LPUB MULTI_STEP ASSEM MODEL_SCALE LOCAL  0.9362`を使う
