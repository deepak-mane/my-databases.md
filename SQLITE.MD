# Sqlite3

##
1. <b>Connect to sample sqlite database file</b>

    Lets work with sqlite database file already present on everyones computer "Cookies"
    - Default location of Cookies on Operating system as below:
    ```
    Window : C:\Users\%USERNAME%\AppData\Local\Google\Chrome\User Data\Default\Cookies
    Linux :
    MOSx :
    ```
    - Naivgate to this location and execute : ``` sqlite3 Cookies```
    - Enter ".help" for usage hints




1. <b></b>
1. <b></b>
1. <b></b>
1. <b></b>
1. <b></b>
1. <b>How to get a list of column names on sqlite3?</b>
```
sqlite> PRAGMA table_info(cookies);
0|creation_utc|INTEGER|1||0
1|host_key|TEXT|1||0
2|name|TEXT|1||0
3|value|TEXT|1||0
4|path|TEXT|1||0
5|expires_utc|INTEGER|1||0
6|is_secure|INTEGER|1||0
7|is_httponly|INTEGER|1||0
8|last_access_utc|INTEGER|1||0
9|has_expires|INTEGER|1|1|0
10|is_persistent|INTEGER|1|1|0
11|priority|INTEGER|1|1|0
12|encrypted_value|BLOB|0|''|0
13|samesite|INTEGER|1|-1|0
sqlite>
```
