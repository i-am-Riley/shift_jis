# 日本語 (シフト JIS) - shift_jis
An older encoding which uses 2 bytes to describe a character. This was added due to the lack of Code Page 932 support for .NET 6.0.

## Usage
- Install from nuget
- Use the following code sample:

```cs
ShiftJISEncoding.GetBytes("てすと"); // will return a byte array with the Shift JIS encoded version of this.
ShiftJISEncoding.GetString(new byte[] { 0x82, 0xC4, 0x82, 0xB7, 0x82, 0xC6 }); // will return a string: てすと
```
