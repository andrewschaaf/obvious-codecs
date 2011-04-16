
# Notation

## ...for images
<pre>
w, h: width, height
x, y:
  ...where the upper-left is (0, 0)
   ...and the lower-right is (w, h)

i = (w * y) + x
</pre>


# Video Codecs

## PD1: pixel-diff-1

### frame\_diff\_body

<pre>
for each differing pixel:
  varint(i_delta) + pixels[i]
</pre>


# Integer Codecs

## varint
<pre>
varint: non-negative integer --> bytes
</pre>

See [Google Protobuf encoding #varints](http://code.google.com/apis/protocolbuffers/docs/encoding.html#varints)

## svarint

See the "Signed Integers" section on that page.