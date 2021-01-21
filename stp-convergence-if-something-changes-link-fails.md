# STP Convergence \(if something changes/link fails\):

Each Non-Root Switch relies on RB's Hello BPDU. If however they fail to receive the Hellos or Hellos lists different details, then Switch starts the convergence process.

* Convergence Process requires the use of 3 Timers:

  \*\*\*\*[**STP** ](https://app.gitbook.com/@mudassirs46/s/network-fundamentals/~/drafts/-MRZ8l67L5MHnaQIEh9W/stp-spanning-tree-protocol)**Timers:**

  | Timer | Default Value | Description |
  | :--- | :--- | :--- |
  | Hello | 2 seconds | Frequency between RB Hello |
  | Max-Age | 10 Times Hello \(20 seconds\) | Convergence process starts after Max-Age timer expires |
  | Forwarding Delay | 15 secs | Delay of 15 seconds in Listening State & 15 Seconds in Learning State after Blocking till Forwarding State |

* If a link fails then by default a Switch receives BPDU every 2 seconds. Then Switch will wait for 20 seconds \(as the max age timer is 10 Hellos \(20 seconds\)\) & then put the port in Listening & Learning State \(again starting the election process\).
* Convergence Process will be completed in 50 seconds as it takes 50 seconds to bring the port up from Blocking to Forwarding Mode. If However the Blocking port & the Forwarding port are on the same link then Switch will understand it's running port went down & will skip the 20 seconds Max-Age timer & immediately start the Forwarding Delay Timer \(Listening + Learning State\)

  **Reference:**

* CCNA 200-301 OCG, Volume 1, Pg. 226- Wendell Odom.
* [https://vimeo.com/ondemand/ccna200301/397383402?autoplay=1](https://vimeo.com/ondemand/ccna200301/397383402?autoplay=1)

