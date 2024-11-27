idf_component_register(SRCS "main.c" "lvgl_demo_ui.c"
                    PRIV_REQUIRES spi_flash esp_driver_gpio esp_driver_spi esp_driver_ledc esp_lcd
                    INCLUDE_DIRS "")
