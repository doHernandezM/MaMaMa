# MaMaMa
*coming soon*

[Device ID (1 byte)] [Part Number (1 byte)] [Total Parts (1 byte)] [Message Type (2 bytes)] [Command/Type (1 byte)] [Value (19 bytes)]



| Group            | Case                    | Command Number | Example of Use (hexadecimal encoding) |
|------------------|-------------------------|----------------|---------------------------------------|
| **System**           | error                   | `0x01`           | `0x01 [Device ID] [Part Number] ...`    |
|                  | lineNumber              | `0x02`           | `0x02 [Device ID] [Part Number] ...`    |
|                  | (space for expansion)   | `0x03-0x0F`      |                                       |
| **Declarations**     | command                 | `0x10`           | `0x10 [Device ID] [Part Number] ...`    |
|                  | comment                 | `0x11`           | `0x11 [Device ID] [Part Number] ...`    |
|                  | operator                | `0x12`           | `0x12 [Device ID] [Part Number] ...`    |
|                  | variable                | `0x13`           | `0x13 [Device ID] [Part Number] ...`    |
|                  | func                    | `0x14`           | `0x14 [Device ID] [Part Number] ...`    |
|                  | varDeclaration          | `0x15`           | `0x15 [Device ID] [Part Number] ...`    |
|                  | space                   | `0x16`           | `0x16 [Device ID] [Part Number] ...`    |
|                  | (space for expansion)   | `0x17-0x1F`      |                                       |
| **Data Types**       | string                  | `0x20`           | `0x20 [Device ID] [Part Number] ...`    |
|                  | int                     | `0x21`           | `0x21 [Device ID] [Part Number] ...`    |
|                  | double                  | `0x22`           | `0x22 [Device ID] [Part Number] ...`    |
|                  | float                   | `0x23`           | `0x23 [Device ID] [Part Number] ...`    |
|                  | bool                    | `0x24`           | `0x24 [Device ID] [Part Number] ...`    |
|                  | (space for expansion)   | `0x25-0x2F`      |                                       |
| **Arithmetic Ops**   | arithmetic              | `0x30`           | `0x30 [Device ID] [Part Number] ...`    |
|                  | (space for expansion)   | `0x31-0x3F`      |                                       |
| **Custom/User**      | userCustom              | `0x40`           | `0x40 [Device ID] [Part Number] ...`    |
| **Commands**         | unassigned              | `0x41`           | `0x41 [Device ID] [Part Number] ...`    |
|                  | print                   | `0x42`           | `0x42 [Device ID] [Part Number] ...`    |
|                  | dev                     | `0x43`           | `0x43 [Device ID] [Part Number] ...`    |
|                  | UI                      | `0x44`           | `0x44 [Device ID] [Part Number] ...`    |
|                  | user                    | `0x45`           | `0x45 [Device ID] [Part Number] ...`    |
|                  | (space for expansion)   | `0x46-0x4F`      |                                       |
| **Operators**        | commentDeclaration      | `0x50`           | `0x50 [Device ID] [Part Number] ...`    |
|                  | letDeclaration          | `0x51`           | `0x51 [Device ID] [Part Number] ...`    |
|                  | varDeclaration          | `0x52`           | `0x52 [Device ID] [Part Number] ...`    |
|                  | funcDeclaration         | `0x53`           | `0x53 [Device ID] [Part Number] ...`    |
|                  | (space for expansion)   | `0x54-0x5F`      |                                       |
| **Logical Ops**      | andOp                   | `0x60`           | `0x60 [Device ID] [Part Number] ...`    |
|                  | orOp                    | `0x61`           | `0x61 [Device ID] [Part Number] ...`    |
|                  | (space for expansion)   | `0x62-0x6F`      |                                       |
| **Comparison Ops**   | lessOp                  | `0x70`           | `0x70 [Device ID] [Part Number] ...`    |
|                  | greaterOp               | `0x71`           | `0x71 [Device ID] [Part Number] ...`    |
|                  | equalsOp                | `0x72`           | `0x72 [Device ID] [Part Number] ...`    |
|                  | (space for expansion)   | `0x73-0x7F`      |                                       |
| **Brackets**         | leftBracket             | `0x80`           | `0x80 [Device ID] [Part Number] ...`    |
|                  | rightBracket            | `0x81`           | `0x81 [Device ID] [Part Number] ...`    |
|                  | (space for expansion)   | `0x82-0x8F`      |                                       |
