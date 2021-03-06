# 4.Snowwhite

Snow White loves her dwarfs, but there are so many and she doesn’t know how to order them. Does she order them by name? Or by the color of their hat? Or by physics? She can’t decide, so it's up to you to write a program that does it for her.

You will be receiving **several input lines** which contain **data** about **dwarfs** in the following format:

"{dwarfName} <:> {dwarfHatColor} <:> {dwarfPhysics}"

The dwarfName and the dwarfHatColor are **strings**. The dwarfPhysics is an **integer**.
You must **store** the **dwarfs** in your program. There are several rules though:

* If **2 dwarfs** have the **same name** but **different colors**, they should be **considered different dwarfs**, and you should store **both** of them.
* If **2 dwarfs** have the **same name** and the **same color**, **store** the **one** with the **higher physics**.

When you receive the command "Once upon a time", the input ends. You must **order** the **dwarfs** by **physics** in **descending order** and then by the **total count** of **dwarfs** with the **same hat color** in **descending order**. Then you must print them all. 

## Input

* The input will consist of **several input lines**, containing **dwarf data** in the format, specified above.
* The input **ends** when you receive the command "Once upon a time". 
## Output

As output, you must print the **dwarfs, ordered** in the way, specified above.
The output format is: "({hatColor}) {name} <-> {physics}"

## Constraints

* The dwarfName will be a **string** that may contain **any ASCII** character except ‘ ’ (space), ‘<’, ‘:’, ‘>’.
* The dwarfHatColor will be a **string** that may contain **any ASCII** character except ‘ ’ (space), ‘<’, ‘:’, ‘>’.
* The dwarfPhysics will be an **integer** in the **range [0, 231 – 1]**.
* There will be **no invalid** input lines.
* If **all sorting criteria fail**, the order should be by **order** of **input.**
* Allowed working **time / memory: 100ms / 16MB**.

## Examples

| Input | Output |
|---|---|
| Peter <:> Red <:> 2000<br>Tony <:> Blue <:> 1000<br>George <:> Green <:> 1000<br>Sam <:> Yellow <:> 4500<br>John <:> Black <:> 1000<br>Once upon a time | (Yellow) Sam <-> 4500<br>(Red) Peter <-> 2000<br>(Blue) Tony <-> 1000<br>(Green) George <-> 1000<br>(Black) John <-> 1000 |
| Peter <:> Red <:> 5000<br>Peter <:> Blue <:> 10000<br>Peter <:> Red <:> 10000<br>George <:> Blue <:> 10000<br>Once upon a time | (Blue) Peter <-> 10000<br>(Blue) George <-> 10000<br>(Red) Peter <-> 10000  |