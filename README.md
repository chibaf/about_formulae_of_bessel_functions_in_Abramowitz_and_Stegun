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

$$
\begin{eqnarray*}
H^{(2)}_{\alpha}(x) \sim \frac{\mathrm{i}}{\pi}e^{-\mathrm{i}x(\sin\tau_0-\tau_0\cos\tau_0)}\left[\frac{\Gamma(\frac{1}{2})}{(\mathrm{i}\frac{x}{2}\sin\tau_0)^{\frac{1}{2}}}-\left(\frac{1}{8}+\frac{5}{24}\cot^2\tau_0\right)\frac{\Gamma(\frac{3}{2})}{(\mathrm{i}\frac{x}{2}\sin\tau_0)^{\frac{3}{2}}}
+\left(\frac{3}{128}+\frac{7}{576}\cot^2\tau_0+\frac{385}{3456}\cot^4\tau_0\right)\frac{\Gamma(\frac{5}{2})}{(\mathrm{i}\frac{x}{2}\sin\tau_0)^{\frac{5}{2}}}+\cdots\right],
% \label{debye-formula: Hankel}
\end{eqnarray*}
$$

where $\tau_0$ is a saddle point and defined through

$$
\begin{equation}
\tau_0=-\mathrm{i}\log\left(\frac{\alpha}{x}+\frac{\alpha}{x}\sqrt{1-\left(\frac{x}{\alpha}\right)^2}\right).
% \label{tau_0}
\end{equation}
$$

Since

$$
\begin{equation*}
\cos\tau_0=\frac{\alpha}{x}, \quad \sin\tau_0=-\mathrm{i}\frac{\alpha}{x}\sqrt{1-\left(\frac{x}{\alpha}\right)^2},
\end{equation*}
$$

we have for a fixed $x>0$

$$
%\begin{eqnarray*}
e^{-\mathrm{i}x(\sin\tau_0-\tau_0\cos\tau_0)}
$$

$$
=\exp\{-\alpha\sqrt{1-(\frac{x}{\alpha})^2}+\alpha\log(\frac{\alpha}{x}+\frac{\alpha}{x}\sqrt{1-(\frac{x}{\alpha})^2})\} 
$$

$$
=\exp(-\alpha\sqrt{1-(\frac{x}{\alpha})^2}) \times (\frac{\alpha}{x}+\frac{\alpha}{x}\sqrt{1-\left(\frac{x}{\alpha})^2})^\alpha
$$

$$
\sim e^{-\alpha} \times (\frac{2\alpha}{x})^\alpha=(\frac{2\alpha}{e x})^\alpha \quad {\rm as}\;\alpha\rightarrow\infty.
%\end{eqnarray*}
$$

On the other hand, the following formulae hold for a fixed $x>0$.

$$
\begin{equation*}
\Gamma\left(\frac{1}{2}\right)=\sqrt{\pi} \quad {\rm and} \quad (\mathrm{i}\frac{x}{2}\sin\tau_0\right)^{1/2} \sim \sqrt{\frac{\alpha}{2}}\quad {\rm as}\;\alpha\rightarrow\infty.
\end{equation*}
$$

Then the first term of (\ref{debye-formula: Hankel}) is asymptotically equal to

$$
\begin{equation*}
\mathrm{i}\sqrt{\frac{2}{\pi\alpha}}(\frac{2\alpha}{e x})^\alpha.
\end{equation*}
$$

Hence we have

$$
\begin{equation*}
H^{(2)}_\alpha(x) \sim \mathrm{i}\sqrt{\frac{2}{\pi\alpha}}\left(\frac{2\alpha}{e x}\right)^\alpha \quad {\rm as}\;\alpha\rightarrow\infty.
\end{equation*}
$$

In the same manner as this discussion, from the following Debye's formula\cite{Debye} we have the asymptotic expansion of $J_\alpha(x)$ for a fixed positive number $x$ as $\alpha\rightarrow\infty$.

$$
\begin{eqnarray}
J_{\alpha}(x)&\sim&\frac{\mathrm{1}}{\pi} e^{\mathrm{i}x(\sin\tau_0-\tau_0\cos\tau_0)}\left[\frac{\Gamma(\frac{1}{2})}{(\mathrm{i}\frac{x}{2}\sin\tau_0)^{\frac{1}{2}}}+\left(\frac{1}{8}+\frac{5}{24}\cot^2\tau_0\right)\frac{\Gamma(\frac{3}{2})}{(\mathrm{i}\frac{x}{2}\sin\tau_0)^{\frac{3}{2}}}\right. \nonumber\\
&&\left.+\left(\frac{3}{128}+\frac{7}{576}\cot^2\tau_0+\frac{385}{3456}\cot^4\tau_0\right)\frac{\Gamma(\frac{5}{2})}{(\mathrm{i}\frac{x}{2}\sin\tau_0)^{\frac{5}{2}}}+\cdots\right],
% \label{debye-formula: Bessel}
\end{eqnarray}
$$

where $\tau_0$ is a saddle point and defined through

$$
\begin{equation}
\tau_0=-\mathrm{i}\log\left(\frac{\alpha}{x}-\frac{\alpha}{x}\sqrt{1-\left(\frac{x}{\alpha}\right)^2}\right).
% \label{tau_0-2}
\end{equation}
% \end{rem}
$$

In this discussion, I use the fact: Bessel funcion is a real part of Hankel function and Neumann function imaginary part in real variable.
