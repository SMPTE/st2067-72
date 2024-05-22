# Public CD of SMPTE ST 2067-72

## General

_This repository is *public*._

Please consult [CONTRIBUTING.md](./CONTRIBUTING.md), [CONFIDENTIALITY.md](./CONFIDENTIALITY.md), [LICENSE.md](./LICENSE.md) and
[PATENTS.md](./PATENTS.md) for important notices.

Please report issues via the repo [Issue Tracker](https://github.com/SMPTE/st2067-72/issues) or at [35pm-chair@smpte.org](mailto:35pm-chair@smpte.org).

## Public Committee Draft (PCD) Notice

The following elements are made available for a public review period ending no earlier than {YYYY-MM-DD}, and no later than {YYYY-MM-DD}:

* [{prose element}]({link to prose element})
* [{element #1}]({link to element #1})
* ...

## Details

The VC-5 codec is a variable-bit-rate codec intended for high-quality video acquisition and post-production and is capable of encoding diverse image and video formats.

The key design goals of the VC-5 codec are:
1. Very high visual quality (visually lossless in most applications),
2. Efficient implementation of both decoders and encoders,
3. Support for any color space or color difference component sampling,
4. Direct encoding of camera sensor output without conversion to a different format, and
5. Adaptability and ease of use in video editing and post-production. 

The VC-5 standards suite comprises the following parts:

**SMPTE ST 2073-1 Elementary Bitstream**</br>
Defines the structure and semantics of a VC-5 bitstream.

**SMPTE RP 2073-2 Conformance Specification**</br>
Specifies the methods for verifying compliance of a bitstream with the VC-5 standards.

**SMPTE ST 2073-3 Image Formats**</br>
Specifies the representation of RGB(A) and YCbCr(A) images and Bayer images as a VC-5 bitstream.

**SMPTE ST 2073-4 Subsampled Color Difference Components**</br>
Specifies the representation of subsampled YCbCr(A) images as a VC-5 bitstream.

**SMPTE ST 2073-5 Layers**</br>
Extends the elementary bitstream syntax with new elements to support the representation of multiple images in a single VC-5 bitstream. Each of the individual images is called a layer. All layers present in the bitstream have the same width, height, number of channels, and image format. For example, a stereo pair can be represented as a single image in the bitstream with a layer for the left image and a layer for right image.

**SMPTE ST 2073-6 Sections**</br>
Extends the VC-5 standards with new elements to support sections that delineate contiguous portions of the bitstream. Sections subdivide the bitstream to enable advanced decoder features such as fast seeking within the bitstream, error detection and correction, multi-resolution decoding, and concurrent decoding.

**SMPTE ST 2073-7 Metadata**</br>
Extends the VC-5 standard to specify a method for representing metadata in VC-5 essence. Metadata as defined in this standard can include intrinsic metadata that is specific to the VC-5 standard, extrinsic metadata that is defined in other standards, and dark metadata in a non-standard format. This standard also defines a method for representing streaming (time series) data in a VC-5 bitstream.

**SMPTE ST 2073-10 Mapping VC-5 Video Essence into the MXF Generic Container**</br>
Specifies the mapping of VC-5 image essence as a picture essence track of the MXF generic container in frame-wrapped, clip-wrapped, or custom-wrapped form.
