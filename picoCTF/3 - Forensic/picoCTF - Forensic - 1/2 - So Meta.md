# So Meta

## Descripción
Find the flag in this [picture](https://challenge-files.picoctf.net/c_fickle_tempest/5efde1f80766d292b7da31469bd46cc06ea5bfa456b2013343e20b64a59e7edc/pico_img.png).

## Solución

```
VictorCervantes-picoctf@webshell:~$ wget https://challenge-files.picoctf.net/c_fickle_tempest/5efde1f80766d292b7da31469bd46cc06ea5bfa456b2013343e20b64a59e7edc/pico_img.png
VictorCervantes-picoctf@webshell:~$ exiftool --version
Syntax:  exiftool [OPTIONS] FILE

Consult the exiftool documentation for a full list of options.
VictorCervantes-picoctf@webshell:~$ exiftool pico_img.png 
ExifTool Version Number         : 12.40
File Name                       : pico_img.png
Directory                       : .
File Size                       : 106 KiB
File Modification Date/Time     : 2025:11:21 19:10:59+00:00
File Access Date/Time           : 2026:03:09 14:12:29+00:00
File Inode Change Date/Time     : 2026:03:09 14:12:29+00:00
File Permissions                : -rw-rw-r--
File Type                       : PNG
File Type Extension             : png
MIME Type                       : image/png
Image Width                     : 600
Image Height                    : 600
Bit Depth                       : 8
Color Type                      : RGB
Compression                     : Deflate/Inflate
Filter                          : Adaptive
Interlace                       : Noninterlaced
Software                        : Adobe ImageReady
XMP Toolkit                     : Adobe XMP Core 5.3-c011 66.145661, 2012/02/06-14:56:27
Creator Tool                    : Adobe Photoshop CS6 (Windows)
Instance ID                     : xmp.iid:A5566E73B2B811E8BC7F9A4303DF1F9B
Document ID                     : xmp.did:A5566E74B2B811E8BC7F9A4303DF1F9B
Derived From Instance ID        : xmp.iid:A5566E71B2B811E8BC7F9A4303DF1F9B
Derived From Document ID        : xmp.did:A5566E72B2B811E8BC7F9A4303DF1F9B
Artist                          : picoCTF{s0_m3ta_b309a657}
Image Size                      : 600x600
Megapixels                      : 0.360
VictorCervantes-picoctf@webshell:~$ 

```

picoCTF{s0_m3ta_b309a657}

## Notas adicionales
- 

## Referencias
- 