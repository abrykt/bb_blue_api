set(SRC_FILES
        adc.c
        bb_blue_api.c
        bb_blue_api.h
        bmp280.c
        board_gpio.c
        board_i2c.c
        board_spi.c
        board_uart.c
        but_led.c
        CMakeLists.txt
        cpu_frequency.c
        dsm2.c
        ehr_pwm.c
        eqep.c
        mpu9250.c
        sensor_config.h
        servo_pru.c
        tipwmss.h
        useful_functions.c
    )

add_library(bb_blue ${SRC_FILES})