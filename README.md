# General
**Execute math expressions in the server or console on PocketMine-MP servers with `/calculator` command**

![EgImg](https://user-images.githubusercontent.com/60387689/199899361-3511a439-e121-42e6-bb65-0d96f7d63196.png)

# Arithmetic Operators
- List of supported arithmetic operators: `/`, `*`, `+`, `-`, `**`, `%`.  
- Description of arithmetic operators: https://github.com/Muqsit/arithmexp/wiki/Operator
- Eg: `/calculator 1 + (2 - 3) * 4 / 5` > Result: `0.2`

# Constants
- List of supported constants: `e`, `euler`, `false`, `inf`, `log2e`, `log10e`, `ln2`, `ln10`, `lnpi`, `pi`, `nan`, `pi2`, `pi4`, `m_1pi`, `m_2pi`, `m_2sqrtpi`, `sqrtpi`, `sqrt2`, `sqrt3`, `sqrt12`, `true`.  
- Description of constants: https://github.com/Muqsit/arithmexp/wiki/Constant
- Eg: `/calculator 3**2 * pi` > Result: `28.2`

# Math functions
- List of supported math functions: `abs()`, `acos()`, `acosh()`, `asin()`, `asinh()`, `atan2()`, `atan()`, `atanh()`, `boolval()`, `ceil()`, `cos()`, `cosh()`, `deg2rad()`, `exp()`, `expm1()`, `fdiv()`, `floatval()`, `floor()`, `fmod()`, `hypot()`, `intdiv()`, `intval()`, `is_bool()`, `is_float()`, `is_finite()`, `is_infinite()`, `is_nan()`, `lcg_value()`, `log10()`, `log1p()`, `log()`, `max()`, `min()`, `mt_getrandmax()`, `mt_rand()`, `pi()`, `pow()`, `rad2deg()`, `round()`, `sin()`, `sinh()`, `sqrt()`, `tan()`, `tanh()`.  
- Description of math functions: https://github.com/Muqsit/arithmexp/wiki/Function
- Eg: `/calculator sqrt(369)` > Result: `19.2`

# Operator
- List of supported operator: `+`, `/`, `==`, `**`, `>`, `>=`, `===`, `<`, `<=`, `&&`, `||`, `and`, `or`, `xor`, `%`, `*`, `!=`, `!==`, `<=>`, `-`, `!`, `-`, `+`.  
- Description of operator: https://github.com/Muqsit/arithmexp/wiki/Operator
- Eg: `/calculator 1 + 2 == 3` > Result: `true`

# Commands & Permissions
```yaml
commands:
  calculator:
    description: "Perform a math operation"
    usage: "/calculator <expression>"
    permission: calculator.command
    aliases: ["calc"]
permissions:
  calculator.command:
    default: true
    description: "Allows the use of /calculator"
```

# Config
```yaml
---
# Prefix of messages.
prefix: "&f[&6Calculator&f]&r"

# {prefix} : Prefix.
# {result} : The result of the math.
result: "{prefix} &aResult: &b{result}"

# {prefix} : Prefix.
# {error} : Error information.
error: "{prefix} &cError: {error}"

# playSound: true > A sound will be sent to the player when a math expressions is performed.
playSound: true

# showDataType: true > The data type will be displayed with the result.
showDataType: true

# Config version
configVersion: "0.0.15"
...


```

# Contact
[![Discord](https://img.shields.io/discord/986553214889517088?label=discord&color=7289DA&logo=discord)](https://discord.gg/j2X83ujT6c)\
**You can contact me directly via Discord `NhanAZ`**
