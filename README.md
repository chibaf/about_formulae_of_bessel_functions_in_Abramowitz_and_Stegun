# about_formulae_of_bessel_functions_in_Abramowitz_and_Stegun
about_formulae_of_bessel_functions_in_Abramowitz_and_Stegun

Abramowitz_and_Stegun shows the following formulae for large $\nu$

asymptotic expansions for bessel functions by order

$$
J_\nu(z) \sim \sqrt{\frac{1}{2\pi\nu}}\left(\frac{ez}{2\nu}\right)^\nu\left[1+O(\nu^{-1})\right], \quad |{\rm arg}\, \nu|<\pi
$$

asymptotic expansions for neumann functions by order

$$
Y_{\nu}(z) \sim -\sqrt{\frac{2}{\pi\nu}}\left(\frac{ez}{2\nu}\right)^{-\nu}\left[1+O(\nu^{-1})\right], \quad |{\rm arg}\, \nu|<\pi
$$

Abramowitz_and_Stegun doesn't note about references of the above formulae

I found Debye's work concerned with these formulae in Iwanami sugaku jiten 4th edition (iwanami mathematical dictionary 4th edition) in Japanese

![1](https://github.com/chibaf/about_formulae_of_bessel_functions_in_Abramowitz_and_Stegun/assets/1296728/96c1f30c-d402-46b4-930d-c7e17fcbdfed)

P. Debye, 
Naeherungsformen fuer Zylinderfunkutionen fuer grrosse werte des Arguments und mbeschraenkt veraederliche werte des Index, Math Ann 67, 535--558 (1909)

Refering Debye's paper, I showed formulae in Abramowitz_and_Stegun as follows.

Using Debye's contour, Debye shows the following asymptotic expansions (\ref{debye-formula: Hankel}) and (\ref{debye-formula: Bessel}) of order $\alpha$ for  $H^{(2)}_{\alpha}(x)$  and  $J_{\alpha}(x)$  from their integral representations\cite{Debye},\cite{Olver1997},\cite{Watson1966}, where $\alpha>x>0$ and  $H^{(2)}_{\alpha}(x)$  is the $\alpha$ th order Hankel function of the second kind. Watson gives an explanation on Debye's contour in his book\cite{Watson1966}.

\begin{eqnarray}
H^{(2)}_{\alpha}(x)&\sim&\frac{\mathrm{i}}{\pi}\e^{-\mathrm{i}x(\sin\tau_0-\tau_0\cos\tau_0)}\left[\frac{\Gamma(\frac{1}{2})}{(\mathrm{i}\frac{x}{2}\sin\tau_0)^{\frac{1}{2}}}-\left(\frac{1}{8}+\frac{5}{24}\cot^2\tau_0\right)\frac{\Gamma(\frac{3}{2})}{(\mathrm{i}\frac{x}{2}\sin\tau_0)^{\frac{3}{2}}}\right. \nonumber\\
&&\left.+\left(\frac{3}{128}+\frac{7}{576}\cot^2\tau_0+\frac{385}{3456}\cot^4\tau_0\right)\frac{\Gamma(\frac{5}{2})}{(\mathrm{i}\frac{x}{2}\sin\tau_0)^{\frac{5}{2}}}+\cdots\right],
\label{debye-formula: Hankel}
\end{eqnarray}

In this discussion, I use the fact: Bessel funcion is a real part of Hankel function and Neumann function imaginary part in real variable.

![1](https://github.com/chibaf/about_formulae_of_bessel_functions_in_Abramowitz_and_Stegun/assets/1296728/a0fcf3a3-e916-477b-81f4-2b1487ae3017)

![In the same manner as this discussion, from the following Dedge's formula(9) we have the](https://github.com/chibaf/about_formulae_of_bessel_functions_in_Abramowitz_and_Stegun/assets/1296728/fa01e087-0da4-474e-a987-b1c58731d04f)
