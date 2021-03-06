WebP Express 0.18.2. Conversion triggered using bulk conversion, 2020-10-23 01:36:26

*WebP Convert 2.3.2*  ignited.
- PHP version: 7.3.22
- Server software: Apache/2.4.46 (Unix) OpenSSL/1.1.1g PHP/7.3.22

Stack converter ignited

Options:
------------
The following options have been set explicitly. Note: it is the resulting options after merging down the "jpeg" and "png" options and any converter-prefixed options.
- source: [doc-root]/wp-content/uploads/2020/10/hero-desktop-768x267.jpg
- destination: [doc-root]/wp-content/uploads/2020/10/hero-desktop-768x267.jpg.webp
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
- source: [doc-root]/wp-content/uploads/2020/10/hero-desktop-768x267.jpg
- destination: [doc-root]/wp-content/uploads/2020/10/hero-desktop-768x267.jpg.webp
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
nice /usr/local/bin/cwebp -metadata all -q 70 -alpha_q '85' -m 6 -low_memory '[doc-root]/wp-content/uploads/2020/10/hero-desktop-768x267.jpg' -o '[doc-root]/wp-content/uploads/2020/10/hero-desktop-768x267.jpg.webp.lossy.webp' 2>&1 2>&1

*Output:* 
Saving file '[doc-root]/wp-content/uploads/2020/10/hero-desktop-768x267.jpg.webp.lossy.webp'
File:      [doc-root]/wp-content/uploads/2020/10/hero-desktop-768x267.jpg
Dimension: 768 x 267
Output:    5370 bytes Y-U-V-All-PSNR 43.85 45.11 43.30   43.94 dB
           (0.21 bpp)
block count:  intra4:        214  (26.23%)
              intra16:       602  (73.77%)
              skipped:       126  (15.44%)
bytes used:  header:            132  (2.5%)
             mode-partition:   1025  (19.1%)
 Residuals bytes  |segment 1|segment 2|segment 3|segment 4|  total
  intra4-coeffs:  |    1886 |      11 |       5 |       9 |    1911  (35.6%)
 intra16-coeffs:  |      14 |       4 |      10 |     202 |     230  (4.3%)
  chroma coeffs:  |    1526 |      14 |      41 |     465 |    2046  (38.1%)
    macroblocks:  |      20%|       2%|       3%|      75%|     816
      quantizer:  |      39 |      37 |      29 |      23 |
   filter level:  |      11 |       8 |       6 |       3 |
------------------+---------+---------+---------+---------+-----------------
 segments total:  |    3426 |      29 |      56 |     676 |    4187  (78.0%)

Success
Reduction: 62% (went from 14 kb to 5 kb)

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
nice /usr/local/bin/cwebp -metadata all -q 70 -alpha_q '85' -near_lossless 60 -m 6 -low_memory '[doc-root]/wp-content/uploads/2020/10/hero-desktop-768x267.jpg' -o '[doc-root]/wp-content/uploads/2020/10/hero-desktop-768x267.jpg.webp.lossless.webp' 2>&1 2>&1

*Output:* 
Saving file '[doc-root]/wp-content/uploads/2020/10/hero-desktop-768x267.jpg.webp.lossless.webp'
File:      [doc-root]/wp-content/uploads/2020/10/hero-desktop-768x267.jpg
Dimension: 768 x 267
Output:    46170 bytes (1.80 bpp)
Lossless-ARGB compressed size: 46170 bytes
  * Header size: 2013 bytes, image data size: 44131
  * Lossless features used: PREDICTION CROSS-COLOR-TRANSFORM SUBTRACT-GREEN
  * Precision Bits: histogram=4 transform=4 cache=10

Success
Reduction: -228% (went from 14 kb to 45 kb)

Picking lossy
cwebp succeeded :)

Converted image in 500 ms, reducing file size with 62% (went from 14 kb to 5 kb)
