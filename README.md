# LieGroupIntegration_with_constraints

## Lie group time integration for constrained systems

The numerical solution of initial value problems for differential equations on manifolds has been considered for about four decades.[^Rheinboldt84] Since the 1990's *Lie group methods* that exploit the specific properties of differentiable manifolds with Lie group structure have found great interest.[^IserlesMuntheKaasNorsettZanna00]

Their practical application in flexible multibody dynamics benefits much from the seminal work of Brüls and Cardona[^BrulsCardona10] who defined and implemented a Lie group generalized-&#945; method for constrained mechanical systems on Lie groups in terms of solution increments in the corresponding Lie algebra.[^BrulsCardonaArnold12] This *Lie algebra approach*[^ArnoldCardonaBruls16] proved to be useful as well in the convergence analysis of these methods[^ArnoldBrulsCardona15] and paved the path for the construction of higher order Lie group BDF methods[^WielochArnold21] and a RATTLE type variational Lie group integrator[^HanteArnold21].

In his recently completed PhD thesis[^Hante22], Hante considered solution increments in the Lie algebra as *derivative vectors* that may be used for a consistent discretization of a geometrically exact beam model in space and time. Part of this work is a comprehensive [open source software repository](https://github.com/StHante) including efficient implementations of

* the Lie group generalized-&#945; method[^BrulsCardona10],
* a second order Lie group BDF method[^WielochArnold21] and
* the variational Lie group integrator RATTLie[^HanteArnold21],[^Hante22]

for the stabilized index-2 formulation of constrained mechanical systems on Lie groups.[^ArnoldCardonaBruls16],[^ArnoldBrulsCardona15] The methods, their implementation and numerical test results are discussed in detail in the PhD thesis[^Hante22]. Furthermore, the GitHub repositories include online documentations. 

In view of [THREAD](https://thread-etn.eu/)'s Deliverable D3.2, the relevant repositories are

* [**gena**](https://github.com/StHante/gena): Lie group generalized-&#945; method,
* [**BLieDF**](https://github.com/StHante/BLieDF): Lie group BDF methods of order $k\leq 2$,
* [**RATTLie**](https://github.com/StHante/RATTLie): RATTLE type variational Lie group integrator,
* [**liegroup**](https://github.com/StHante/liegroup): basic components of Lie group integrators like exponential map, tangent operator, ... ,
* [**heavy_top**](https://github.com/StHante/heavy_top): benchmark problem Heavy Top[^BrulsCardona10].

[^ArnoldBrulsCardona15]: M. Arnold, O. Brüls, and A. Cardona: Error analysis of generalized-&#945; Lie group time integration methods for constrained mechanical systems. *Numerische Mathematik* **129**(2015)149-179. [https://doi.org/10.1007/s00211-014-0633-1](https://doi.org/10.1007/s00211-014-0633-1)

[^ArnoldCardonaBruls16]: M. Arnold, A. Cardona, and O. Brüls: A Lie algebra approach to Lie group time integration of constrained systems. In P. Betsch, editor, *Structure-Preserving Integrators in Nonlinear Structural Dynamics and Flexible Multibody Dynamics*, volume 565 of *CISM Courses and Lectures*, pages 91-158. Springer International Publishing, Cham, 2016. [https://doi.org/10.1007/978-3-319-31879-0_3](https://doi.org/10.1007/978-3-319-31879-0_3)

[^BrulsCardona10]: O. Brüls and A. Cardona: On the use of Lie group time integrators in multibody dynamics. *J. Comput. Nonlinear Dynam.* **5**(2010)031002 (13 pages). [https://doi.org/10.1115/1.4001370](https://doi.org/10.1115/1.4001370)

[^BrulsCardonaArnold12]: O. Brüls, A. Cardona, and M. Arnold: Lie group generalized-&#945; time integration of constrained flexible multibody systems. *Mechanism and Machine Theory* **48**(2012)121-137. [https://doi.org/10.1016/j.mechmachtheory.2011.07.017](https://doi.org/10.1016/j.mechmachtheory.2011.07.017)

[^Hante22]: S. Hante: *Geometric Integration of a Constrained Cosserat Beam Model*. PhD thesis, Martin Luther University Halle-Wittenberg, Institute of Mathematics, June 2022. [https://doi.org/10.25673/91397](https://doi.org/10.25673/91397)

[^HanteArnold21]: S. Hante and M. Arnold: RATTLie: A variational Lie group integration scheme for constrained mechanical systems. *Journal of Computational and Applied Mathematics* **387**(2021):112492 (14 pages). [https://doi.org/10.1016/j.cam.2019.112492](https://doi.org/10.1016/j.cam.2019.112492)

[^IserlesMuntheKaasNorsettZanna00]: A. Iserles, H.Z. Munthe-Kaas, S. Nørsett, and A. Zanna: Lie-group methods. *Acta Numerica* **9**(2000)215-365. [https://doi.org/10.1017/S0962492900002154](https://doi.org/10.1017/S0962492900002154)

[^Rheinboldt84]: W.C. Rheinboldt: Differential-algebraic systems as differential equations on  manifolds. *Math. Comp.* **43**(1984)473-482. [https://doi.org/10.1090/S0025-5718-1984-0758195-5](https://doi.org/10.1090/S0025-5718-1984-0758195-5)

[^WielochArnold21]: V. Wieloch and M. Arnold: BDF integrators for constrained mechanical systems on Lie groups. *Journal of Computational and Applied Mathematics* **387**(2021)112517 (17 pages). [https://doi.org/10.1016/j.cam.2019.112517](https://doi.org/10.1016/j.cam.2019.112517)
