# Snapshot report for `test/prefer-math-trunc.js`

The actual snapshot is saved in `prefer-math-trunc.js.snap`.

Generated by [AVA](https://avajs.dev).

## prefer-math-trunc - #01

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = 1.1 | 0;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(1.1);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = 1.1 | 0;␊
        |             ^^^^^^^ Use `Math.trunc` instead of `| 0`.␊
    `

## prefer-math-trunc - #02

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = 111 | 0;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(111);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = 111 | 0;␊
        |             ^^^^^^^ Use `Math.trunc` instead of `| 0`.␊
    `

## prefer-math-trunc - #03

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = (1 + 2 / 3.4) | 0;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(1 + 2 / 3.4);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = (1 + 2 / 3.4) | 0;␊
        |             ^^^^^^^^^^^^^^^^^ Use `Math.trunc` instead of `| 0`.␊
    `

## prefer-math-trunc - #04

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = bar((1.4 | 0) + 2);␊
    ␊
    Output:␊
      1 | const foo = bar((Math.trunc(1.4)) + 2);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = bar((1.4 | 0) + 2);␊
        |                  ^^^^^^^ Use `Math.trunc` instead of `| 0`.␊
    `

## prefer-math-trunc - #05

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = (0, 1.4) | 0;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc((0, 1.4));␊
    ␊
    Error 1/1:␊
    > 1 | const foo = (0, 1.4) | 0;␊
        |             ^^^^^^^^^^^^ Use `Math.trunc` instead of `| 0`.␊
    `

## prefer-math-trunc - #06

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = 1.4 | 0.;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(1.4);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = 1.4 | 0.;␊
        |             ^^^^^^^^ Use `Math.trunc` instead of `| 0.`.␊
    `

## prefer-math-trunc - #07

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = 1.4 | .0;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(1.4);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = 1.4 | .0;␊
        |             ^^^^^^^^ Use `Math.trunc` instead of `| .0`.␊
    `

## prefer-math-trunc - #08

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = 1.4 | 0.0000_0000_0000;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(1.4);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = 1.4 | 0.0000_0000_0000;␊
        |             ^^^^^^^^^^^^^^^^^^^^^^ Use `Math.trunc` instead of `| 0.0000_0000_0000`.␊
    `

## prefer-math-trunc - #09

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = 1.4 | 0b0;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(1.4);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = 1.4 | 0b0;␊
        |             ^^^^^^^^^ Use `Math.trunc` instead of `| 0b0`.␊
    `

## prefer-math-trunc - #10

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = 1.4 | 0x0000_0000_0000;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(1.4);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = 1.4 | 0x0000_0000_0000;␊
        |             ^^^^^^^^^^^^^^^^^^^^^^ Use `Math.trunc` instead of `| 0x0000_0000_0000`.␊
    `

## prefer-math-trunc - #11

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = 1.4 | 0o0;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(1.4);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = 1.4 | 0o0;␊
        |             ^^^^^^^^^ Use `Math.trunc` instead of `| 0o0`.␊
    `

## prefer-math-trunc - #12

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = 1.23 | 0 | 4;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(1.23) | 4;␊
    ␊
    Error 1/1:␊
    > 1 | const foo = 1.23 | 0 | 4;␊
        |             ^^^^^^^^ Use `Math.trunc` instead of `| 0`.␊
    `

## prefer-math-trunc - #13

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = ~~3.9;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(3.9);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = ~~3.9;␊
        |             ^^^^^ Use `Math.trunc` instead of `~~`.␊
    `

## prefer-math-trunc - #14

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = ~~111;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(111);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = ~~111;␊
        |             ^^^^^ Use `Math.trunc` instead of `~~`.␊
    `

## prefer-math-trunc - #15

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = ~~(1 + 2 / 3.4);␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(1 + 2 / 3.4);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = ~~(1 + 2 / 3.4);␊
        |             ^^^^^^^^^^^^^^^ Use `Math.trunc` instead of `~~`.␊
    `

## prefer-math-trunc - #16

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = ~~1 + 2 / 3.4;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(1) + 2 / 3.4;␊
    ␊
    Error 1/1:␊
    > 1 | const foo = ~~1 + 2 / 3.4;␊
        |             ^^^ Use `Math.trunc` instead of `~~`.␊
    `

## prefer-math-trunc - #17

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = ~~(0, 1.4);␊
    ␊
    Output:␊
      1 | const foo = Math.trunc((0, 1.4));␊
    ␊
    Error 1/1:␊
    > 1 | const foo = ~~(0, 1.4);␊
        |             ^^^^^^^^^^ Use `Math.trunc` instead of `~~`.␊
    `

## prefer-math-trunc - #18

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = ~~~10.01;␊
    ␊
    Output:␊
      1 | const foo = ~Math.trunc(10.01);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = ~~~10.01;␊
        |              ^^^^^^^ Use `Math.trunc` instead of `~~`.␊
    `

## prefer-math-trunc - #19

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = ~~(~10.01);␊
    ␊
    Output:␊
      1 | const foo = ~Math.trunc(10.01);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = ~~(~10.01);␊
        |              ^^^^^^^^^ Use `Math.trunc` instead of `~~`.␊
    `

## prefer-math-trunc - #20

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = ~(~~10.01);␊
    ␊
    Output:␊
      1 | const foo = ~(Math.trunc(10.01));␊
    ␊
    Error 1/1:␊
    > 1 | const foo = ~(~~10.01);␊
        |               ^^^^^^^ Use `Math.trunc` instead of `~~`.␊
    `

## prefer-math-trunc - #21

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = ~~-10.01;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(-10.01);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = ~~-10.01;␊
        |             ^^^^^^^^ Use `Math.trunc` instead of `~~`.␊
    `

## prefer-math-trunc - #22

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = ~~~~10.01;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(Math.trunc(10.01));␊
    ␊
    Error 1/1:␊
    > 1 | const foo = ~~~~10.01;␊
        |               ^^^^^^^ Use `Math.trunc` instead of `~~`.␊
    `

## prefer-math-trunc - #23

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = 10.01 >> 0;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(10.01);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = 10.01 >> 0;␊
        |             ^^^^^^^^^^ Use `Math.trunc` instead of `>> 0`.␊
    `

## prefer-math-trunc - #24

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = 10.01 << 0;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(10.01);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = 10.01 << 0;␊
        |             ^^^^^^^^^^ Use `Math.trunc` instead of `<< 0`.␊
    `

## prefer-math-trunc - #25

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = 10.01 ^ 0;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(10.01);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = 10.01 ^ 0;␊
        |             ^^^^^^^^^ Use `Math.trunc` instead of `^ 0`.␊
    `

## prefer-math-trunc - #26

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = {a: {b: {c: 3}}};␊
      2 | const bar = a.b.c | 0;␊
    ␊
    Output:␊
      1 | const foo = {a: {b: {c: 3}}};␊
      2 | const bar = Math.trunc(a.b.c);␊
    ␊
    Error 1/1:␊
      1 | const foo = {a: {b: {c: 3}}};␊
    > 2 | const bar = a.b.c | 0;␊
        |             ^^^^^^^^^ Use `Math.trunc` instead of `| 0`.␊
    `

## prefer-math-trunc - #27

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = {a: {b: {c: 3}}};␊
      2 | const bar = a.b?.c | 0;␊
    ␊
    Output:␊
      1 | const foo = {a: {b: {c: 3}}};␊
      2 | const bar = Math.trunc(a.b?.c);␊
    ␊
    Error 1/1:␊
      1 | const foo = {a: {b: {c: 3}}};␊
    > 2 | const bar = a.b?.c | 0;␊
        |             ^^^^^^^^^^ Use `Math.trunc` instead of `| 0`.␊
    `

## prefer-math-trunc - #28

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = {a: {b: {c: 3}}};␊
      2 | const bar = ~~a.b?.c;␊
    ␊
    Output:␊
      1 | const foo = {a: {b: {c: 3}}};␊
      2 | const bar = Math.trunc(a.b?.c);␊
    ␊
    Error 1/1:␊
      1 | const foo = {a: {b: {c: 3}}};␊
    > 2 | const bar = ~~a.b?.c;␊
        |             ^^^^^^^^ Use `Math.trunc` instead of `~~`.␊
    `

## prefer-math-trunc - #29

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = 3;␊
      2 | const bar = foo | 0;␊
    ␊
    Output:␊
      1 | const foo = 3;␊
      2 | const bar = Math.trunc(foo);␊
    ␊
    Error 1/1:␊
      1 | const foo = 3;␊
    > 2 | const bar = foo | 0;␊
        |             ^^^^^^^ Use `Math.trunc` instead of `| 0`.␊
    `

## prefer-math-trunc - #30

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = 3;␊
      2 | const bar = ~~foo;␊
    ␊
    Output:␊
      1 | const foo = 3;␊
      2 | const bar = Math.trunc(foo);␊
    ␊
    Error 1/1:␊
      1 | const foo = 3;␊
    > 2 | const bar = ~~foo;␊
        |             ^^^^^ Use `Math.trunc` instead of `~~`.␊
    `

## prefer-math-trunc - #31

> Snapshot 1

    `␊
    Input:␊
      1 | let foo = 2;␊
      2 | foo |= 0;␊
    ␊
    Output:␊
      1 | let foo = 2;␊
      2 | foo = Math.trunc(foo);␊
    ␊
    Error 1/1:␊
      1 | let foo = 2;␊
    > 2 | foo |= 0;␊
        | ^^^^^^^^ Use `Math.trunc` instead of `|= 0`.␊
    `

## prefer-math-trunc - #32

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = {a: {b: 3.4}};␊
      2 | foo.a.b |= 0;␊
    ␊
    Output:␊
      1 | const foo = {a: {b: 3.4}};␊
      2 | foo.a.b = Math.trunc(foo.a.b);␊
    ␊
    Error 1/1:␊
      1 | const foo = {a: {b: 3.4}};␊
    > 2 | foo.a.b |= 0;␊
        | ^^^^^^^^^^^^ Use `Math.trunc` instead of `|= 0`.␊
    `

## prefer-math-trunc - #33

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = 10.01;␊
      2 | const bar = ~~foo;␊
    ␊
    Output:␊
      1 | const foo = 10.01;␊
      2 | const bar = Math.trunc(foo);␊
    ␊
    Error 1/1:␊
      1 | const foo = 10.01;␊
    > 2 | const bar = ~~foo;␊
        |             ^^^^^ Use `Math.trunc` instead of `~~`.␊
    `

## prefer-math-trunc - #34

> Snapshot 1

    `␊
    Input:␊
      1 | let foo = 10.01;␊
      2 | foo >>= 0;␊
    ␊
    Output:␊
      1 | let foo = 10.01;␊
      2 | foo = Math.trunc(foo);␊
    ␊
    Error 1/1:␊
      1 | let foo = 10.01;␊
    > 2 | foo >>= 0;␊
        | ^^^^^^^^^ Use `Math.trunc` instead of `>>= 0`.␊
    `

## prefer-math-trunc - #35

> Snapshot 1

    `␊
    Input:␊
      1 | let foo = 10.01;␊
      2 | foo <<= 0;␊
    ␊
    Output:␊
      1 | let foo = 10.01;␊
      2 | foo = Math.trunc(foo);␊
    ␊
    Error 1/1:␊
      1 | let foo = 10.01;␊
    > 2 | foo <<= 0;␊
        | ^^^^^^^^^ Use `Math.trunc` instead of `<<= 0`.␊
    `

## prefer-math-trunc - #36

> Snapshot 1

    `␊
    Input:␊
      1 | let foo = 10.01;␊
      2 | foo ^= 0;␊
    ␊
    Output:␊
      1 | let foo = 10.01;␊
      2 | foo = Math.trunc(foo);␊
    ␊
    Error 1/1:␊
      1 | let foo = 10.01;␊
    > 2 | foo ^= 0;␊
        | ^^^^^^^^ Use `Math.trunc` instead of `^= 0`.␊
    `

## prefer-math-trunc - #37

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = /* first comment */ 3.4 | 0; // A B C␊
    ␊
    Output:␊
      1 | const foo = /* first comment */ Math.trunc(3.4); // A B C␊
    ␊
    Error 1/1:␊
    > 1 | const foo = /* first comment */ 3.4 | 0; // A B C␊
        |                                 ^^^^^^^ Use `Math.trunc` instead of `| 0`.␊
    `

## prefer-math-trunc - #38

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = /* first comment */ ~~3.4; // A B C␊
    ␊
    Output:␊
      1 | const foo = /* first comment */ Math.trunc(3.4); // A B C␊
    ␊
    Error 1/1:␊
    > 1 | const foo = /* first comment */ ~~3.4; // A B C␊
        |                                 ^^^^^ Use `Math.trunc` instead of `~~`.␊
    `

## prefer-math-trunc - #39

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = {a: {b: 3.4}};␊
      2 | foo /* Comment 1 */ .a /* Comment 2 */ . /* Comment 3 */ b |= /* Comment 4 */ 0 /* Comment 5 */;␊
    ␊
    Output:␊
      1 | const foo = {a: {b: 3.4}};␊
      2 | foo /* Comment 1 */ .a /* Comment 2 */ . /* Comment 3 */ b = Math.trunc(foo /* Comment 1 */ .a /* Comment 2 */ . /* Comment 3 */ b) /* Comment 5 */;␊
    ␊
    Error 1/1:␊
      1 | const foo = {a: {b: 3.4}};␊
    > 2 | foo /* Comment 1 */ .a /* Comment 2 */ . /* Comment 3 */ b |= /* Comment 4 */ 0 /* Comment 5 */;␊
        | ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ Use `Math.trunc` instead of `|= 0`.␊
    `

## prefer-math-trunc - #40

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = {a: {b: 3.4}};␊
      2 | const bar = /* Comment 1 */ ~~ a /* Comment 3 */ . /* Comment 4 */ b /* Comment 5 */;␊
    ␊
    Output:␊
      1 | const foo = {a: {b: 3.4}};␊
      2 | const bar = /* Comment 1 */ Math.trunc(a /* Comment 3 */ . /* Comment 4 */ b) /* Comment 5 */;␊
    ␊
    Error 1/1:␊
      1 | const foo = {a: {b: 3.4}};␊
    > 2 | const bar = /* Comment 1 */ ~~ a /* Comment 3 */ . /* Comment 4 */ b /* Comment 5 */;␊
        |                             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ Use `Math.trunc` instead of `~~`.␊
    `

## prefer-math-trunc - #41

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = /* will keep */ 3.4 /* will remove 1 */ | /* will remove 2 */ 0;␊
    ␊
    Output:␊
      1 | const foo = /* will keep */ Math.trunc(3.4);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = /* will keep */ 3.4 /* will remove 1 */ | /* will remove 2 */ 0;␊
        |                             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ Use `Math.trunc` instead of `| 0`.␊
    `

## prefer-math-trunc - #42

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = /* will keep */ ~ /* will remove 1 */ ~ /* will remove 2 */ 3.4;␊
    ␊
    Output:␊
      1 | const foo = /* will keep */ Math.trunc(3.4);␊
    ␊
    Error 1/1:␊
    > 1 | const foo = /* will keep */ ~ /* will remove 1 */ ~ /* will remove 2 */ 3.4;␊
        |                             ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ Use `Math.trunc` instead of `~~`.␊
    `

## prefer-math-trunc - #43

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = 3.4; // comment 1␊
      2 | foo |= 0; // comment 2␊
    ␊
    Output:␊
      1 | const foo = 3.4; // comment 1␊
      2 | foo = Math.trunc(foo); // comment 2␊
    ␊
    Error 1/1:␊
      1 | const foo = 3.4; // comment 1␊
    > 2 | foo |= 0; // comment 2␊
        | ^^^^^^^^ Use `Math.trunc` instead of `|= 0`.␊
    `

## prefer-math-trunc - #44

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = 3.4; // comment 1␊
      2 | const bar = ~~foo; // comment 2␊
    ␊
    Output:␊
      1 | const foo = 3.4; // comment 1␊
      2 | const bar = Math.trunc(foo); // comment 2␊
    ␊
    Error 1/1:␊
      1 | const foo = 3.4; // comment 1␊
    > 2 | const bar = ~~foo; // comment 2␊
        |             ^^^^^ Use `Math.trunc` instead of `~~`.␊
    `

## prefer-math-trunc - #45

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = ~~10.01 | 0;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(Math.trunc(10.01));␊
    ␊
    Error 1/2:␊
    > 1 | const foo = ~~10.01 | 0;␊
        |             ^^^^^^^^^^^ Use `Math.trunc` instead of `| 0`.␊
    Error 2/2:␊
    > 1 | const foo = ~~10.01 | 0;␊
        |             ^^^^^^^ Use `Math.trunc` instead of `~~`.␊
    `

## prefer-math-trunc - #46

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = ~~(10.01 | 0);␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(Math.trunc(10.01));␊
    ␊
    Error 1/2:␊
    > 1 | const foo = ~~(10.01 | 0);␊
        |             ^^^^^^^^^^^^^ Use `Math.trunc` instead of `~~`.␊
    Error 2/2:␊
    > 1 | const foo = ~~(10.01 | 0);␊
        |                ^^^^^^^^^ Use `Math.trunc` instead of `| 0`.␊
    `

## prefer-math-trunc - #47

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = 10.01 | 0 | 0;␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(Math.trunc(10.01));␊
    ␊
    Error 1/2:␊
    > 1 | const foo = 10.01 | 0 | 0;␊
        |             ^^^^^^^^^^^^^ Use `Math.trunc` instead of `| 0`.␊
    Error 2/2:␊
    > 1 | const foo = 10.01 | 0 | 0;␊
        |             ^^^^^^^^^ Use `Math.trunc` instead of `| 0`.␊
    `

## prefer-math-trunc - #48

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = ~~~~((10.01 | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
    ␊
    Output:␊
      1 | const foo = Math.trunc(Math.trunc(Math.trunc(Math.trunc(Math.trunc(Math.trunc(Math.trunc(Math.trunc(Math.trunc(Math.trunc(10.01))))))))));␊
    ␊
    Error 1/9:␊
    > 1 | const foo = ~~~~((10.01 | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
        |               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ Use `Math.trunc` instead of `~~`.␊
    Error 2/9:␊
    > 1 | const foo = ~~~~((10.01 | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
        |                  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ Use `Math.trunc` instead of `^ 0`.␊
    Error 3/9:␊
    > 1 | const foo = ~~~~((10.01 | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
        |                  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ Use `Math.trunc` instead of `^ 0`.␊
    Error 4/9:␊
    > 1 | const foo = ~~~~((10.01 | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
        |                  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ Use `Math.trunc` instead of `<< 0`.␊
    Error 5/9:␊
    > 1 | const foo = ~~~~((10.01 | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
        |                  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^ Use `Math.trunc` instead of `<< 0`.␊
    Error 6/9:␊
    > 1 | const foo = ~~~~((10.01 | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
        |                  ^^^^^^^^^^^^^^^^^^^^^^^^^ Use `Math.trunc` instead of `>> 0`.␊
    Error 7/9:␊
    > 1 | const foo = ~~~~((10.01 | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
        |                  ^^^^^^^^^^^^^^^^^^^^ Use `Math.trunc` instead of `>> 0`.␊
    Error 8/9:␊
    > 1 | const foo = ~~~~((10.01 | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
        |                   ^^^^^^^^^^^^^ Use `Math.trunc` instead of `| 0`.␊
    Error 9/9:␊
    > 1 | const foo = ~~~~((10.01 | 0 | 0) >> 0 >> 0 << 0 << 0 ^ 0 ^0);␊
        |                   ^^^^^^^^^ Use `Math.trunc` instead of `| 0`.␊
    `

## prefer-math-trunc - #49

> Snapshot 1

    `␊
    Input:␊
      1 | const foo = Array.from({length: 10}, (_, index) => (index + 1) + (index + 1) /100);␊
      2 | let i = 0;␊
      3 | while (i < foo.length) {␊
      4 | 	foo[i++] |= 0;␊
      5 | }␊
      6 | console.log(foo);␊
    ␊
    Output:␊
    [Same as input]␊
    ␊
    Error 1/1:␊
      1 | const foo = Array.from({length: 10}, (_, index) => (index + 1) + (index + 1) /100);␊
      2 | let i = 0;␊
      3 | while (i < foo.length) {␊
    > 4 | 	foo[i++] |= 0;␊
        | 	^^^^^^^^^^^^^ Use `Math.trunc` instead of `|= 0`.␊
      5 | }␊
      6 | console.log(foo);␊
    `