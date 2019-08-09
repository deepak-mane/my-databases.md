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

1. <b>List Schema/Tables</b>
    ```.tables```
1. <b>How to get a list of column names on one of table from sqlite3?</b>
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
1. <b>How to Select rows from table matching one of column name?</b>
```
sqlite> select * from cookies where host_key like '%bloom%';
13209825680869535|.bloombergbusiness.com|sailthru_bid||/|13209836853486722|0|0|13209826053486722|1|1|1||-1
13209825680869448|.bloombergbusiness.com|sailthru_hid||/|13241382979486615|0|0|13209826053486615|1|1|1||-1
13209826551460047|.bloomberg.com|__gads||/|14838251499000000|0|0|13209830018637463|1|1|1||-1
13209826553188588|.bloomberg.com|_csrf||/|0|1|1|13209830076637220|0|0|1||-1
13209826553067470|.bloomberg.com|_gcl_au||/|13217602553000000|0|0|13209830018637463|1|1|1||-1
13209826553093967|.bloomberg.com|_user-status||/|0|0|0|13209830018637463|0|0|1||-1
13209826553300186|.bloomberg.com|_user_newsletters||/|0|0|0|13209830018637463|0|0|1||-1
13209826554005919|.www.bloomberg.com|bb_geo_info||/|13241362554000000|0|0|13209830018637463|1|1|1||-1
sqlite>

```
1. <b></b>
1. <b></b>
1. <b></b>
