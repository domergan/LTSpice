Solution of exercise 2.2 of The Art of Electronics, pp. 78 (Third Edition):

The right side of $$C_1$$ (Q2’s base) makes an RC circuit that rises toward $$+5\text{ V}$$ through $$R_3$$ after being lowered to $$-4.4\text{ V}$$.
With $$R_3C_1=\tau=10\text{k}\cdot10\text{ nF}=100~\mu\text{s}$$,

$$
V_b(t)=V_\infty+(V_0-V_\infty)e^{-t/\tau}
=5+(-4.4-5)e^{-t/\tau}=5-9.4e^{-t/\tau}.
$$

The pulse ends when $$V_b(t)$$ reaches the B-E turn-on of Q2 ($$\approx0.6\text{ V}$$, $$\approx0.7\text{ V}$$ for the 2N2222*):

$$
0.6=5-9.4e^{-t/\tau}
\;\Rightarrow\;
e^{-t/\tau}=\frac{5-0.6}{9.4}=\frac{4.4}{9.4}
\;\Rightarrow\;
t=\tau\ln\!\left(\frac{9.4}{4.4}\right).
$$

$$
t \approx 0.759\,\tau \approx 0.759(100~\mu\text{s}) \approx 75.9~\mu\text{s}\approx 0.76\,RC.
$$

So $$T_{\text{pulse}}\approx 0.76R_3C_1\approx 76~\mu\text{s}$$.
