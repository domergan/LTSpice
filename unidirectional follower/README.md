With a diode inside the feedback path, the loop cancels the diode drop whenever current flows from the op-amp to the load. This circuit forms the basis of circuits like peak detectors.

#### Conduction ($$V_{\text{IN}} > V_{\text{OUT}}$$)

The diode forward-biases and the loop closes. The op-amp drives so that:

$$
V_{\text{OUT}} \approx V_{\text{IN}},\qquad
V_{\text{INT}} \approx V_{\text{IN}} + V_F
$$

The drop $$V_F$$ appears across the diode, not between IN and OUT.

#### Blocking ($$V_{\text{IN}} < V_{\text{OUT}}$$)

The diode is reverse-biased and the loop opens. The op-amp saturates low, but that doesn’t affect OUT because the diode is off. OUT is then set by the load/leakage. With no load, OUT floats when the diode opens (it “holds” the last value).
