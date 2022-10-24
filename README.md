# Compression and Decompression for Arduino

Unishox is a technique for compressing short strings.  This library provides for Arduino the same API as the desktop version at [Unishox - Guaranteed compression for Short Strings](https://github.com/siara-cc/Unishox).

To find out how Unishox works, read [this article](https://github.com/siara-cc/Unishox/blob/master/Unishox_Article_2.pdf?raw=true).

## Usage

The following API can be used for compressing and decompressing strings or files:

```
int unishox_compress_simple(const char *in, long len, char *out);
int unishox_decompress_simple(const char *in, long len, char *out);
```

See example provided for demonstration of usage or see the documentation at https://github.com/siara-cc/Unishox for further details.

For using Unishox to store compressed data in Progmem of Arduino Uno and up, see the library at https://github.com/siara-cc/Unishox_Arduino_Progmem_lib.

## Example

The example provided with this library allows you to enter a string and see how much compression can be achieved.  In general, compression utilities such as `zip`, `gzip` do not compress short strings well and often expand them.  They also use lots of memory which makes them unusable in constrained environments like Arduino.

## Related projects

- [Storing compressed text in Arduino Flash memory](https://github.com/siara-cc/Unishox_Arduino_Progmem_lib)
- [Unishox Sqlite3 User Defined Function as loadable extension](https://github.com/siara-cc/Unishox_Sqlite_UDF)
- [Sqlite3 Library for ESP32](https://github.com/siara-cc/esp32_arduino_sqlite3_lib)
- [Sqlite3 Library for ESP8266](https://github.com/siara-cc/esp_arduino_sqlite3_lib)
- [Sqlite3 Library for ESP-IDF](https://github.com/siara-cc/esp32-idf-sqlite3)
