[![General Assembly Logo](https://camo.githubusercontent.com/1a91b05b8f4d44b5bbfb83abac2b0996d8e26c92/687474703a2f2f692e696d6775722e636f6d2f6b6538555354712e706e67)](https://generalassemb.ly/education/web-development-immersive)

# Air Traffic Control Challenge

## Prerequisites

-   [ga-wdi-boston/js-objects-stack-challenge](https://github.com/ga-wdi-boston/js-objects-stack-challenge)

## Instructions

1.  Fork and clone this repository.
1.  Change into the new directory.
1.  Create and checkout a new branch to work on.
  1.  Write your code in [`lib/atc.js`](lib/atc.js)
1.  Fulfill the listed requirements.

## Requirements

A software subsystem of an air-traffic control system is defined to manage a
queue of aircraft (AC) in an airport. Write a constructor function, `AtcQueue`,
that creates an aircraft queue.

The aircraft queue is managed by a
process which responds to three types of requests:

  - Enqueue aircraft used to insert a new AC into the system. `enqueue`
  - Dequeue aircraft used to remove an AC from the system. `dequeue`
  - AircraftCount used to count the aircraft in the queue. `aircraftCount`

AC have at least (but are not limited to having) the following properties:

  - AC `type`: passenger or cargo.
  - AC `size`: small or large.

The process which manages the queue of AC satisfies the following:

  - There is no limit on the number of AC it can manage.
  - Dequeue aircraft requests result in selection of one AC for removal such
    that:
    - Passenger AC have removal precedence over Cargo AC.
    - Large AC of a given type have removal precedence over Small AC of the
      same type.
    - Earlier enqueued AC of a given type and size have precedence over later
      enqueued AC of the same type and size.

Use `grunt test` to test your code.

## [License](LICENSE)

1.  All content is licensed under a CC­BY­NC­SA 4.0 license.
1.  All software code is licensed under GNU GPLv3. For commercial use or
    alternative licensing, please contact legal@ga.co.
