## Unix-Rice 

Configurations and dotfiles for my Desktop themes and shortcuts. 

### Firefox Setup
- Go to `about:config`  
- set `True` for `toolkit.tabbox.switchByScrolling`
- set `False` for `ui.key.menuAccessKeyFocuses`

### Sublime Text Build 3211
- Go to `Preferences` -> `Settings` and add the following:
```
{
	"update_check": false,
	"font": 14
}
```
- 3211 https://gist.github.com/OrionUnix/51ae230f5f9ea6c332b5639f556cc1d6
```
----- BEGIN LICENSE -----
Member J2TeaM
Single User License
EA7E-1011316
D7DA350E 1B8B0760 972F8B60 F3E64036
B9B4E234 F356F38F 0AD1E3B7 0E9C5FAD
FA0A2ABE 25F65BD8 D51458E5 3923CE80
87428428 79079A01 AA69F319 A1AF29A4
A684C2DC 0B1583D4 19CBD290 217618CD
5653E0A0 BACE3948 BB2EE45E 422D2C87
DD9AF44B 99C49590 D2DBDEE1 75860FD2
8C8BB2AD B2ECE5A4 EFC08AF2 25A9B864
------ END LICENSE ------
```
- 4126 https://gist.github.com/skoqaq/3f3e8f28e23c881143cef9cf49d821ff
```
—– BEGIN LICENSE —–
Mifeng User
Single User License
EA7E-1184812
C0DAA9CD 6BE825B5 FF935692 1750523A
EDF59D3F A3BD6C96 F8D33866 3F1CCCEA
1C25BE4D 25B1C4CC 5110C20E 5246CC42
D232C83B C99CCC42 0E32890C B6CBF018
B1D4C178 2F9DDB16 ABAA74E5 95304BEF
9D0CCFA9 8AF8F8E2 1E0A955E 4771A576
50737C65 325B6C32 817DCB83 A7394DFA
27B7E747 736A1198 B3865734 0B434AA5
—— END LICENSE ——
```

### Delete Boot Menu
- https://unix.stackexchange.com/questions/552728/removed-both-linux-installations-but-bios-still-shows-them-in-boot-options
- `bcdedit /enum firmware`
- `bcdedit /delete <identifier>`
