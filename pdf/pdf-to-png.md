```
convert -quality 100 -density 300 input.pdf output.png
```

```
gs -dSAFER -dBATCH -dNOPAUSE -dNOPROMPT -dMaxBitmap=500000000 -dEPSCrop -dAlignToPixels=0 -dGridFitTT=2 -sDEVICE=pngalpha -dTextAlphaBits=4 -dGraphicsAlphaBits=4 -dUseCIEColor -r72x72 -sOUTPUTFILE=output.png input.eps
```
