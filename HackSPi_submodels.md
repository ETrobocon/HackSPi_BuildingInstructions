# HackSPi Building Instruction
## LPub3D settings, DON'T USE NATIVE RENDERER! 
### Configuration->Preferences->Renderers->Preferred renderer: LDView
### ~/LDView->Renderer Settings->LDView Preferences->Geometry->Edge Lines->Thickness: 3(center)

# Zeta Platforms submodel structure

## ReHackSM6
Re-Hacks (ZetaRefined) ETRR25ZM6
- **ReHackSM6_FrontChassis**
    - **ReHackSM6_Body**
        - ZetaShooterConcept_Head
        - HackSPi_DachsM5_Arm
            - HackSPi_DachsM5_ColorSensor
    - HackSPi_DachsM6_WholeMotor
        - HackSPi_DachsM5_LeftMotorJoint
        - HackSPi_DachsM5_RightMotorJoint
        - HackSPi_DachsM6_LeftMotor
            - ZetaChariotConcept_Motor25Z
        - HackSPi_DachsM6_RightMotor
            - ZetaChariotConcept_Motor25Z
        - HackSPi_DachsM5_ArmGearSupport
    - HackSPi_DachsM5_Apillar
        - HackSPi_DachsM5_ArmGear
    - ZetaShooterConcept_ApillarBodyJoint
    - HackSPi_DachsM5_FrontChassisJoint
- **ReHackSM6_RearChassis**
    - **ReHackSM6_TouchSensor**
    - EpsilonSpikerConcept_RearChassisJoint

## HackSPi_DachsM6
HackSPi dachs (ZetaShooter) ETR25ZM6
- **HackSPi_DachsM6_FrontChassis**
    - HackSPi_DachsM5_Body
        - HackSPi_DachsM5_Head
        - HackSPi_DachsM5_Arm
            - HackSPi_DachsM5_ColorSensor
    - HackSPi_DachsM5_FrontCamera
    - **HackSPi_DachsM6_WholeMotor**
        - HackSPi_DachsM5_LeftMotorJoint
        - HackSPi_DachsM5_RightMotorJoint
        - **HackSPi_DachsM6_LeftMotor**
            - ZetaChariotConcept_Motor25Z
        - **HackSPi_DachsM6_RightMotor**
            - ZetaChariotConcept_Motor25Z
        - HackSPi_DachsM5_ArmGearSupport
    - HackSPi_DachsM5_Apillar
        - HackSPi_DachsM5_ArmGear
    - ZetaShooterConcept_ApillarBodyJoint
    - HackSPi_DachsM5_FrontChassisJoint
- HackSPi_DachsM5_RearChassis
    - HackSPi_DachsM5_Caster
    - EpsilonSpikerConcept_RearChassisJoint
    - HackSPi_DachsM5_Cpillar
    - HackSPi_DachsM5_Bpillar
    - HackSPi_DachsM5_TouchSensor
- HackSPi_DachsM5_LeftUpperApillarBpillarJoint
- HackSPi_DachsM5_RightUpperApillarBpillarJoint
- HackSPi_DachsM5_LeftUnderApillarBpillarJoint
- HackSPi_DachsM5_RightUnderApillarBpillarJoint
- HackSPi_DachsM5_AdjustableWeight

## HackSPi_DachsM5
HackSPi dachs (ZetaShooter) ETR25ZM5
- **HackSPi_DachsM5_FrontChassis**
    - **HackSPi_DachsM5_Body**
        - **HackSPi_DachsM5_Head**
        - **HackSPi_DachsM5_Arm**
            - **HackSPi_DachsM5_ColorSensor**
    - **HackSPi_DachsM5_FrontCamera**
    - **HackSPi_DachsM5_WholeMotor**
        - **HackSPi_DachsM5_LeftMotorJoint**
        - **HackSPi_DachsM5_RightMotorJoint**
        - **HackSPi_DachsM5_LeftMotor**
            - ZetaChariotConcept_Motor25Z
        - **HackSPi_DachsM5_RightMotor**
            - ZetaChariotConcept_Motor25Z
        - **HackSPi_DachsM5_ArmGearSupport**
    - **HackSPi_DachsM5_Apillar**
        - **HackSPi_DachsM5_ArmGear**
    - ZetaShooterConcept_ApillarBodyJoint
    - **HackSPi_DachsM5_FrontChassisJoint**
- **HackSPi_DachsM5_RearChassis**
    - **HackSPi_DachsM5_Caster**
    - EpsilonSpikerConcept_RearChassisJoint
    - **HackSPi_DachsM5_Cpillar**
        - ~~**HackSPi_DachsM5_RearCamera~~
    - **HackSPi_DachsM5_Bpillar**
    - **HackSPi_DachsM5_TouchSensor**
- **HackSPi_DachsM5_LeftUpperApillarBpillarJoint**
- **HackSPi_DachsM5_RightUpperApillarBpillarJoint**
- **HackSPi_DachsM5_LeftUnderApillarBpillarJoint**
- **HackSPi_DachsM5_RightUnderApillarBpillarJoint**
- **HackSPi_DachsM5_AdjustableWeight**

## ZZetaShooterConcept
ZZetaShooter Concept ETR40ZZM4/80ZZM4 "HackSPi Tabby"
- **ZZetaShooterConcept_FrontChassis**
    - **ZZetaShooterConcept_Body**
        - ZetaShooterConcept_Head
        - **ZZetaShooterConcept_Camera**
            - **ZZetaShooterConcept_CameraStay**
            - **ZZetaShooterConcept_CameraSupport**
        - **ZZetaShooterConcept_Arm**
    - **ZZetaShooterConcept_ArmGear**
    - **ZetaShooterConcept_WholeMotor**
        - **ZetaShooterConcept_LeftMotor**
            - ZetaChariotConcept_Motor25Z
        - **ZetaShooterConcept_RightMotor**
            - ZetaChariotConcept_Motor25Z
        - **ZZetaShooterConcept_Wheel**
            - EpsilonSpikerConcept_WheelCap
    - ZetaChariotConcept_ApillarBodyJoint
    - EpsilonSpikerConcept_FrontChassisJoint
- **ZZetaShooterConcept_RearChassis**
    - **ZZetaShooterConcept_Caster**
    - **ZZetaShooterConcept_CasterSupport**
    - **ZZetaShooterConcept_RearChassisJoint**
    - **ZZetaShooterConcept_Bpillar**
- EpsilonSpikerConcept_RearChassisApillarJoint
- **ZZetaShooterConcept_LeftUpperApillarBpillarJoint**
- **ZZetaShooterConcept_RightUpperApillarBpillarJoint**
- **ZZetaShooterConcept_LeftUnderApillarBpillarJoint**
- **ZZetaShooterConcept_RightUnderApillarBpillarJoint**
- **ZZetaShooterConcept_BatterySupport**


## ZetaShooterConcept
ZetaShooter Concept ETR25ZM4/50ZM4 "HackSPi Dax"
- **ZetaShooterConcept_FrontChassis**
    - **ZetaShooterConcept_Body**
        - **ZetaShooterConcept_Head**
        - **ZetaShooterConcept_Camera**
    - **ZetaShooterConcept_Arm**
        - **ZetaShooterConcept_ColorSensor**
    - **ZetaShooterConcept_ArmGear**
    - **ZetaShooterConcept_WholeMotor**
        - **ZetaShooterConcept_LeftMotor**
        - **ZetaShooterConcept_RightMotor**
    - **ZetaShooterConcept_ApillarBodyJoint**
    - EpsilonSpikerConcept_FrontChassisJoint
- **ZetaShooterConcept_RearChassis**
    - **ZetaShooterConcept_Caster**
    - EpsilonSpikerConcept_RearChassisJoint
    - **ZetaShooterConcept_Bpillar**
    - **ZetaShooterConcept_LeftRearChassisBCpillarJoint**
    - **ZetaShooterConcept_RightRearChassisBCpillarJoint**
    - **ZetaShooterConcept_TouchSensor**
- **ZetaShooterConcept_LeftApillarBpillarJoint**
- **ZetaShooterConcept_RightApillarBpillarJoint**
- **ZetaShooterConcept_BatterySupport**

## ZZetaInvaderConcept
ZZetaInvader Concept ETR80ZZIM4
- **ZZetaInvaderConcept_Camera**
- **ZZetaInvaderConcept_LeftCameraMount**
- **ZZetaInvaderConcept_RightCameraMount**

## ZZetaSpikerConcept
ZZetaSpiker Concept ETR40ZZSM4
- ZetaChariotConcept_Head
- **ZetaSpikerConcept_Arm**
- **ZetaSpikerConcept_ArmGear**
- **ZetaSpikerConcept_ArmMotor**
- ZetaChariotConcept_TouchSensor
- ZetaChariotConcept_Apillar
- ZetaChariotConcept_ApillarBodyJoint
- ZZetaChariotConcept_Motor40ZZ

## ZetaChariotConcept / ZZetaChariotConcept
Zeta/ZZetaChariot Concept ETR25ZCM4~80ZZCM4
- **ZZetaChariotConcept_RearChassis**
    - **ZetaChariotConcept_Head**
    - **ZetaChariotConcept_TouchSensor**
    - **ZetaChariotConcept_ColorSensor**
    - **ZetaChariotConcept_Apillar**
    - **ZetaChariotConcept_ApillarBodyJoint**
    - **ZetaChariotConcept_Motor25Z**
    - **ZetaChariotConcept_Motor50Z**
    - **ZZetaChariotConcept_Motor40ZZ**
    - **ZZetaChariotConcept_Motor80ZZ**
- **ZetaChariotConcept_FrontChassis**
    - **ZetaChariotConcept_LeftArm**
    - **ZetaChariotConcept_RightArm**
    - **ZetaChariotConcept_CameraMount**
- **ZetaChariotConcept_LeftFrontRearJoint**
- **ZetaChariotConcept_RightFrontRearJoint**


# HackSPi submodel structure

## HackSPi_M4_Arrow
HackSPi (EpsilonSpiker) ETR50EPM4
- **HackSPi_M4_FrontChassis_Arrow**
    - HackSPi_M2_ArmMotor_Arrow
        - EpsilonSpikerConcept_LightSensor_Arrow
        - HackSPi_M2_BumperSpacer_Arrow
    - **HackSPi_M4_Apillar_Arrow**
        - ~~HackSPi_M2_BatterySupport_Arrow~~
        - EpsilonSpikerConcept_RasPiSupport
        - ~~HackSPi_M2_MagentaCableClip_Arrow~~
        - EpsilonSpikerConcept_Roof_Arrow
    - HackSPi_M2_FrontChassisJoint_Arrow
    - **HackSPi_M4_SpikeHub_Arrow**
    - ~~EpsilonSpikerConcept_Head_Arrow~~
        - ~~EpsilonSpikerConcept_Antenna_Arrow~~
    - HackSPi_M2_Wheel_Arrow
        - HackSPi_M2_WheelCap_Arrow
- HackSPi_M2_RearChassis_Arrow
    - EpsilonSpikerConcept_Caster_Arrow
    - EpsilonSpikerConcept_RearChassisJoint_Arrow
- EpsilonSpikerConcept_RearChassisApillarJoint_Arrow
- ~~EpsilonSpikerConcept_Cpillar_GroundCamera_Arrow~~
    - ~~EpsilonSpikerConcept_CameraModule_Arrow~~
- **HackSPi_M4_Cpillar**
- EpsilonSpikerConcept_LeftRearChassisCpillarJoint_Arrow
- EpsilonSpikerConcept_RightRearChassisCpillarJoint_Arrow
- ~~EpsilonSpikerConcept_LeftApillarCpillarJoint_Arrow~~
- ~~EpsilonSpikerConcept_RightApillarCpillarJoint_Arrow~~
- **HackSPi_M4_LeftNeck**
- **HackSPi_M4_RightNeck**
- **HackSPi_M4_Head**
    - **HackSPi_M4_CameraModule**


## HackSPi_M4
HackSPi Clione (EpsilonPredator) ETR50EPM4
- **HackSPi_M4_FrontChassis**
    - EpsilonSpikerConcept_ArmMotor
        - EpsilonSpikerConcept_LightSensor
    - **HackSPi_M4_Apillar**
        - EpsilonSpikerConcept_RasPiSupport
        - **HackSPi_M4_LeftRoof**
        - **HackSPi_M4_RightRoof**
    - EpsilonSpikerConcept_FrontChassisJoint
    - **HackSPi_M4_SpikeHub**
    - EpsilonSpikerConcept_Wheel
        - EpsilonSpikerConcept_WheelCap
- HackSPi_M2_RearChassis
    - EpsilonSpikerConcept_Caster
    - EpsilonSpikerConcept_RearChassisJoint
- EpsilonSpikerConcept_RearChassisApillarJoint
- **HackSPi_M4_Cpillar**
- EpsilonSpikerConcept_LeftRearChassisCpillarJoint
- EpsilonSpikerConcept_RightRearChassisCpillarJoint
- **HackSPi_M4_LeftNeck**
- **HackSPi_M4_RightNeck**
- **HackSPi_M4_Head**
    - **HackSPi_M4_CameraModule**


## HackSPi_M2
HackSPi (EpsilonSpiker) ETR50ESM2
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
- **HackSPi_M2_RearChassis**
    - EpsilonSpikerConcept_Caster
    - EpsilonSpikerConcept_RearChassisJoint
- EpsilonSpikerConcept_RearChassisApillarJoint
- EpsilonSpikerConcept_Cpillar_GroundCamera
    - EpsilonSpikerConcept_CameraModule
- EpsilonSpikerConcept_LeftRearChassisCpillarJoint
- EpsilonSpikerConcept_RightRearChassisCpillarJoint
- EpsilonSpikerConcept_LeftApillarCpillarJoint
- EpsilonSpikerConcept_RightApillarCpillarJoint


## HackSPi_M2_Arrow
HackSPi (EpsilonSpiker) ETR50ESM2
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
EpsilonSpiker Concept ETR50ESM1
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
