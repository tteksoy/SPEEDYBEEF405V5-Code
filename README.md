# SPEEDYBEEF405V5-Code
https://github.com/iNavFlight/inav/pull/11059#issuecomment-4029817584

https://github.com/cluez0r/inav/commit/0b6a166e87e02be9094f56dbab5c85d3ad1d7c18

https://github.com/iNavFlight/inav/compare/master...cluez0r:inav:speedybeef405v5


 git clone https://github.com/iNavFlight/inav
 
Fix I2C1 ports

target.c

    DEF_TIM(TIM3,   CH4, PB1,  TIM_USE_MOTOR, 1, 0), // S1 (PB1/TIM3_CH4)
    
    DEF_TIM(TIM3,   CH3, PB0,  TIM_USE_MOTOR, 1, 0), // S2 (PB0/TIM3_CH3)
    
    DEF_TIM(TIM2,   CH3, PB10, TIM_USE_MOTOR, 1, 0), // S3 (PB10/TIM2_CH3)
    
    DEF_TIM(TIM2,   CH4, PB11, TIM_USE_MOTOR, 1, 1), // S4 (PB11/TIM2_CH4)
    
    DEF_TIM(TIM8,   CH4, PC9,  TIM_USE_SERVO, 1, 0), // S5 (PC9/TIM8_CH4)
    
    DEF_TIM(TIM8,   CH3, PC8,  TIM_USE_SERVO, 1, 0), // S6 (PC8/TIM8_CH3)
    
    DEF_TIM(TIM2,   CH3, PB10, TIM_USE_OUTPUT_AUTO, 1, 0), // S7
    
    DEF_TIM(TIM2,   CH1, PA15, TIM_USE_OUTPUT_AUTO, 1, 0), // S8
    


target.h

// *************** I2C(Baro & I2C) **************************

#define USE_I2C

#define USE_I2C_DEVICE_1

#define I2C1_SCL                PB6

#define I2C1_SDA                PB7


