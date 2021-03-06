WebP Express 0.18.2. Conversion triggered using bulk conversion, 2020-10-23 01:36:25

*WebP Convert 2.3.2*  ignited.
- PHP version: 7.3.22
- Server software: Apache/2.4.46 (Unix) OpenSSL/1.1.1g PHP/7.3.22

Stack converter ignited

Options:
------------
The following options have been set explicitly. Note: it is the resulting options after merging down the "jpeg" and "png" options and any converter-prefixed options.
- source: [doc-root]/wp-content/uploads/2020/10/hero-tablet.jpg
- destination: [doc-root]/wp-content/uploads/2020/10/hero-tablet.jpg.webp
- log-call-arguments: true
- converters: (array of 9 items)

The following options have not been explicitly set, so using the following defaults:
- converter-options: (empty array)
- shuffle: false
- preferred-converters: (empty array)
- extra-converters: (empty array)

The following options were supplied and are passed on to the converters in the stack:
- encoding: "auto"
- metadata: "all"
- near-lossless: 60
- quality: 70
------------


*Trying: cwebp* 

Options:
------------
The following options have been set explicitly. Note: it is the resulting options after merging down the "jpeg" and "png" options and any converter-prefixed options.
- source: [doc-root]/wp-content/uploads/2020/10/hero-tablet.jpg
- destination: [doc-root]/wp-content/uploads/2020/10/hero-tablet.jpg.webp
- encoding: "auto"
- low-memory: true
- log-call-arguments: true
- metadata: "all"
- method: 6
- near-lossless: 60
- quality: 70
- use-nice: true
- command-line-options: ""
- try-common-system-paths: true
- try-supplied-binary-for-os: true

The following options have not been explicitly set, so using the following defaults:
- alpha-quality: 85
- auto-filter: false
- default-quality: 75
- max-quality: 85
- preset: "none"
- size-in-percentage: null (not set)
- skip: false
- rel-path-to-precompiled-binaries: *****
- try-cwebp: true
- try-discovering-cwebp: true
------------

Encoding is set to auto - converting to both lossless and lossy and selecting the smallest file

Converting to lossy
Looking for cwebp binaries.
Discovering if a plain cwebp call works (to skip this step, disable the "try-cwebp" option)
- Executing: cwebp -version 2>&1. Result: *Exec failed* (the cwebp binary was not found at path: cwebp)
Nope a plain cwebp call does not work
Discovering binaries using "which -a cwebp" command. (to skip this step, disable the "try-discovering-cwebp" option)
Found 0 binaries
Discovering binaries by peeking in common system paths (to skip this step, disable the "try-common-system-paths" option)
Found 1 binaries: 
- /usr/local/bin/cwebp
Discovering binaries which are distributed with the webp-convert library (to skip this step, disable the "try-supplied-binary-for-os" option)
Checking if we have a supplied precompiled binary for your OS (Darwin)... We do.
Found 1 binaries: 
- [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-103-mac-10_14
Detecting versions of the cwebp binaries found
- Executing: /usr/local/bin/cwebp -version 2>&1. Result: version: *1.1.0*
- Executing: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-103-mac-10_14 -version 2>&1. Result: *Exec failed*. Permission denied (user: "d4all" does not have permission to execute that binary)
Binaries ordered by version number.
- /usr/local/bin/cwebp: (version: 1.1.0)
Trying the first of these. If that should fail (it should not), the next will be tried and so on.
Creating command line options for version: 1.1.0
Quality: 70. 
Consider setting quality to "auto" instead. It is generally a better idea
The near-lossless option ignored for lossy
Trying to convert by executing the following command:
nice /usr/local/bin/cwebp -metadata all -q 70 -alpha_q '85' -m 6 -low_memory '[doc-root]/wp-content/uploads/2020/10/hero-tablet.jpg' -o '[doc-root]/wp-content/uploads/2020/10/hero-tablet.jpg.webp.lossy.webp' 2>&1 2>&1

*Output:* 
Saving file '[doc-root]/wp-content/uploads/2020/10/hero-tablet.jpg.webp.lossy.webp'
File:      [doc-root]/wp-content/uploads/2020/10/hero-tablet.jpg
Dimension: 1536 x 800
Output:    17580 bytes Y-U-V-All-PSNR 46.58 46.65 45.25   46.34 dB
           (0.11 bpp)
block count:  intra4:        931  (19.40%)
              intra16:      3869  (80.60%)
              skipped:      2488  (51.83%)
bytes used:  header:            160  (0.9%)
             mode-partition:   5721  (32.5%)
 Residuals bytes  |segment 1|segment 2|segment 3|segment 4|  total
  intra4-coeffs:  |    4609 |      60 |      18 |      27 |    4714  (26.8%)
 intra16-coeffs:  |      56 |      19 |      14 |     427 |     516  (2.9%)
  chroma coeffs:  |    5150 |     203 |      71 |    1018 |    6442  (36.6%)
    macroblocks:  |      18%|       2%|       2%|      78%|    4800
      quantizer:  |      39 |      37 |      31 |      23 |
   filter level:  |      16 |      23 |       5 |       3 |
------------------+---------+---------+---------+---------+-----------------
 segments total:  |    9815 |     282 |     103 |    1472 |   11672  (66.4%)
Metadata:
  * EXIF data:        68 bytes

Success
Reduction: 84% (went from 106 kb to 17 kb)

Converting to lossless
Looking for cwebp binaries.
Discovering if a plain cwebp call works (to skip this step, disable the "try-cwebp" option)
- Executing: cwebp -version 2>&1. Result: *Exec failed* (the cwebp binary was not found at path: cwebp)
Nope a plain cwebp call does not work
Discovering binaries using "which -a cwebp" command. (to skip this step, disable the "try-discovering-cwebp" option)
Found 0 binaries
Discovering binaries by peeking in common system paths (to skip this step, disable the "try-common-system-paths" option)
Found 1 binaries: 
- /usr/local/bin/cwebp
Discovering binaries which are distributed with the webp-convert library (to skip this step, disable the "try-supplied-binary-for-os" option)
Checking if we have a supplied precompiled binary for your OS (Darwin)... We do.
Found 1 binaries: 
- [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-103-mac-10_14
Detecting versions of the cwebp binaries found
- Executing: /usr/local/bin/cwebp -version 2>&1. Result: version: *1.1.0*
- Executing: [doc-root]/wp-content/plugins/webp-express/vendor/rosell-dk/webp-convert/src/Convert/Converters/Binaries/cwebp-103-mac-10_14 -version 2>&1. Result: *Exec failed*. Permission denied (user: "d4all" does not have permission to execute that binary)
Binaries ordered by version number.
- /usr/local/bin/cwebp: (version: 1.1.0)
Trying the first of these. If that should fail (it should not), the next will be tried and so on.
Creating command line options for version: 1.1.0
Trying to convert by executing the following command:
nice /usr/local/bin/cwebp -metadata all -q 70 -alpha_q '85' -near_lossless 60 -m 6 -low_memory '[doc-root]/wp-content/uploads/2020/10/hero-tablet.jpg' -o '[doc-root]/wp-content/uploads/2020/10/hero-tablet.jpg.webp.lossless.webp' 2>&1 2>&1

*Output:* 
Saving file '[doc-root]/wp-content/uploads/2020/10/hero-tablet.jpg.webp.lossless.webp'
File:      [doc-root]/wp-content/uploads/2020/10/hero-tablet.jpg
Dimension: 1536 x 800
Output:    215402 bytes (1.40 bpp)
Lossless-ARGB compressed size: 215402 bytes
  * Header size: 5279 bytes, image data size: 210097
  * Lossless features used: PREDICTION CROSS-COLOR-TRANSFORM SUBTRACT-GREEN
  * Precision Bits: histogram=5 transform=4 cache=10
Metadata:
  * EXIF data:        68 bytes

Success
Reduction: -98% (went from 106 kb to 210 kb)

Picking lossy
cwebp succeeded :)

Converted image in 1772 ms, reducing file size with 84% (went from 106 kb to 17 kb)
