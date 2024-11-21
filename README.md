## Dependencies

### External Libraries:
- `lvgl`
- `esp_lcd_ili9341`

### Internal Libraries:
- `esp_driver_gpio`
- `esp_driver_spi`
- `esp_driver_ledc`
- `esp_lcd`

---

## Wiring

The following are the pin configurations for the display and other components.

```c
// LCD Pixel Clock Frequency
#define EXAMPLE_LCD_PIXEL_CLOCK_HZ     (20 * 1000 * 1000) // 20 MHz

// Backlight Control Levels
#define EXAMPLE_LCD_BK_LIGHT_ON_LEVEL  1
#define EXAMPLE_LCD_BK_LIGHT_OFF_LEVEL !EXAMPLE_LCD_BK_LIGHT_ON_LEVEL

// Pin Definitions
#define EXAMPLE_PIN_NUM_SCLK           18  // SPI Clock Pin
#define EXAMPLE_PIN_NUM_MOSI           23  // SPI MOSI Pin
#define EXAMPLE_PIN_NUM_MISO           19  // SPI MISO Pin
#define EXAMPLE_PIN_NUM_LCD_DC         21  // LCD Data/Command Pin
#define EXAMPLE_PIN_NUM_LCD_RST        22  // LCD Reset Pin
#define EXAMPLE_PIN_NUM_LCD_CS         5   // LCD Chip Select Pin
#define EXAMPLE_PIN_NUM_BK_LIGHT       2   // Backlight Pin
#define EXAMPLE_PIN_NUM_TOUCH_CS       15  // Touch Controller Chip Select Pin
