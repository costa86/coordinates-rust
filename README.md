# Coordinates

A CLI tool to get distance (km) between 2 coordinates
  
|Linux|Windows  |
|--|--|
|./coordinates | coordinates.exe |

## 1. Algorithm used
[Haversine formula](https://en.wikipedia.org/wiki/Haversine_formula)

## 2. Usage

    Gets the distance (km) between two coordinates using Haversine formula

    USAGE:
        coordinates --first <LATITUDE,LONGITUDE> --second <LATITUDE,LONGITUDE>

    OPTIONS:
        -f, --first <LATITUDE,LONGITUDE>     Comma-separated latitude 1 and longitude 1
        -h, --help                           Print help information
        -s, --second <LATITUDE,LONGITUDE>    Comma-separated latitude 2 and longitude 2
        -V, --version      

## 3. Example

| Place | Latitude| Longitude  |
|--|--|--|
| Paris | 48.85341 | -2.34880 |
| London | 51.50853 | -0.12574 |


```sh
./coordinates -f 48.85341,-2.34880 -s 51.50853,-0.12574
```

```sh
335.0
```
> Coordinates' ranges :warning:
>
> -90 <= latitude <= 90
>
> -180 <= longitude <= 180
