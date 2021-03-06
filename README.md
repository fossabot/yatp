# yatp
Yet another thread pool in Rust that is adaptive, responsive and generic.

_It is still a work in progress._

[![Build Status](https://travis-ci.org/tikv/yatp.svg?branch=master)](https://travis-ci.org/tikv/yatp)
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Ftikv%2Fyatp.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Ftikv%2Fyatp?ref=badge_shield)

## Features

* **Adaptive**: Yatp adjusts the number of working threads automatically. Under
  light workloads, unnecessary context switches are greatly reduced.

* **Responsive**: Yatp supports different kinds of task queues with advanced
  scheduling algorithms like [multi-level feedback queue][MLFQ].

* **Generic**: Yatp is easily adapted to various tasks. Simple callbacks,
  [futures 0.1] and [std Future] are built-in supported.

[MLFQ]: https://en.wikipedia.org/wiki/Multilevel_feedback_queue
[futures 0.1]: https://docs.rs/futures/0.1.*/futures/future/trait.Future.html
[std Future]: https://doc.rust-lang.org/stable/std/future/trait.Future.html


## License
[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Ftikv%2Fyatp.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Ftikv%2Fyatp?ref=badge_large)