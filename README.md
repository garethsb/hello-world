# hello-world
repo to test 2FA
first commit...
<a name="mark-1">
</a>
more stuff

yet more <a name="mark-2"></a> stuff

and <a name="mark-3">yet more stuff again</a>
but isn't that enough stuff now?

n<sub>1</sub> / d<sub>1</sub>

`n<sub>1</sub> / d<sub>1</sub>`

`n`<sub>`1`</sub>` / d`<sub>`1`</sub>

_n<sub>1</sub> * d<sub>2</sub>_ and _n<sub>2</sub> * d<sub>1</sub>_

| A | B |
|---|---|
|a<br>a<br>a|b<br>b<br>b|

<table>
<tr>
<td> Status </td> <td> Response </td>
</tr>
<tr>
<td>

200

</td>
<td>

<table>
<tr><th>Receiver Caps</th><th>Query API - RQL</th></tr>
<tr><td>

```json
{
  ...
  "transport": "urn:x-nmos:transport:rtp",
  "format": "urn:x-nmos:format:video",
  "caps": {
    "media_types": [ "video/raw" ],
    "version": "1603796863:314159275",
    "constraint_sets": [
      {
        "urn:x-nmos:cap:meta:label": "1080i",
        "urn:x-nmos:cap:format:color_sampling": {
          "enum": [ "YCbCr-4:2:2" ]
        },
        "urn:x-nmos:cap:format:frame_height": {
          "enum": [ 1080 ]
        },
        "urn:x-nmos:cap:format:frame_width": {
          "enum": [ 1920 ]
        },
        "urn:x-nmos:cap:format:grain_rate": {
          "enum": [
             { "numerator": 25 },
             { "numerator": 30000, "denominator": 1001 }
           ]
        },
        "urn:x-nmos:cap:format:interlace_mode": {
          "enum": [
            "interlaced_tff",
            "interlaced_bff",
            "interlaced_psf"
          ]
        }
      },
      {
        "urn:x-nmos:cap:meta:label": "1080p",
        "urn:x-nmos:cap:format:color_sampling": {
          "enum": [ "YCbCr-4:2:2" ]
        },
        "urn:x-nmos:cap:format:frame_height": {
          "enum": [ 1080 ]
        },
        "urn:x-nmos:cap:format:frame_width": {
          "enum": [ 1920 ]
        },
        "urn:x-nmos:cap:format:grain_rate": {
          "enum": [
             { "numerator": 25 },
             { "numerator": 30000, "denominator": 1001 },
             { "numerator": 50 },
             { "numerator": 60000, "denominator": 1001 }
           ]
        },
        "urn:x-nmos:cap:format:interlace_mode": {
          "enum": [ "progressive" ]
        }
      }
    ]
  }
}
```

</td>
<td>

```
/x-nmos/query/v1.3/flows/?query.rql=and(


  eq(format,urn%3ax-nmos%3aformat%3avideo),

  in(media_type,(video%2fraw)),

 or(
    and(

      eq(components,sampling:YCbCr-4%3a2%3a2),


      eq(frame_height,1080),


      eq(frame_width,1920),



      in(grain_rate,(
        rational:25%2f1,
        rational:30000%2f1001
      )),


      in(interlace_mode,(
        interlaced_tff,
        interlaced_bff,
        interlaced_psf
      ))

    ),
    and(

      eq(components,sampling:YCbCr-4%3a2%3a2),


      eq(frame_height,1080),


      eq(frame_width,1920),



      in(grain_rate,(
        rational:25%2f1,
        rational:30000%2f1001,
        rational:50%2f1,
        rational:60000%2f1001
      )),

      eq(interlace_mode,progressive)


    )
  )

)
```

</td></tr>
</table>

```json
{
    "username": "garethsb",
    "answer": 42,
    "dat": true
}
```

</td>
</tr>
<tr>
<td>

400

</td>
<td>

**Markdown** _here_. (Blank lines needed before and after!)

</td>
</tr>
</table>
