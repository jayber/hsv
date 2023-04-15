# hsv

![Codecov](https://img.shields.io/codecov/c/github/jayber/hsv)

### Simple conversion of HSV color space to RGB

A simple function [hsv_to_rgb](/src/lib.rs) to convert values in the HSV color space to RGB. I 
created this crate
because I couldn't find an existing one that worked for me, and, when I asked chatGPT how to convert
HSV to RGB in Rust, it pointed me to a crate called hsv that didn't exist. Now it does.


### Instructions

* One function `hsv_to_rgb` taking `hue: f64, saturation: f64, value: f64` and returning `u8, u8,
  u8`
* Panics if supplied values is not within allowed ranges: 0 - 360, 0 - 1, 0 - 1 respectively
* May not be correct in some sense, but should be okay for simple use cases.
* Based mostly on https://en.wikipedia.org/wiki/HSL_and_HSV#Color_conversion_formulae

[Please let me know if it's incorrect. Bug reports and PRs welcome!](https://github.com/jayber/hsv)