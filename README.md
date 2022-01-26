# Nigerian State, Capital, Cities and Geolocations!


## Inspiration
The have been several times I have needed to use Nigeria states, cities in my project and i have to check several repositories to find what I am looking for. So I have decided to make a repository that will have everything you need about Nigerian states/cities et.c.
My real motivation is to be also able to have each state mapped out with their respective Geolocation (in points and location) using [GeoJSON](https://datatracker.ietf.org/doc/html/rfc7946) format.


## File descriptions

> All files mentioned here can be found in the `lib` folder and they all have a `.min.json` copy which is minified.

`nigeria-state-and-capital.json` contains all Nigeria's state and capital.
A single record will return a JSON that looks like below



`nigeria-state-and-geolocation.json` contains all Nigeria's states and capitals with the state code, state's geometric boundaries, and state's centroid (the geometric centre).

 > N.B: The centroid doesnt necessarily means it will be the capital city as most capitals are not necessarily in the state's centre

A single record will return a JSON that looks like below

```json
  {
        "state": "Lagos",
        "state_code": "LA",
        "centroid": {
            "type": "Point",
            "coordinates": [
                3.5774005,
                6.5269033
            ]
        },
        "geometry": {
            "type": "Polygon",
            "coordinates": [
                [
                    [
                        2.7059846,
                        6.4212932
                    ],
                   // ...truncated for brevity
                ]
            ]
        },
        "capital": "Ikeja"
    }
```

## Found an issue?

You can reach out to me via email officialwebdev[at]gmail.com

## Want to contribute?

Just make a fork, and make a PR, which will be reviewed. If all looks well, it's going to be merged.
