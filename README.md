<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/minif-logotype-dark.svg">
    <img src="assets/minif-logotype.svg" alt="MinIF" width="340">
  </picture>
</p>

<p align="center">
  <b>Optimizing dynamic information flow control with a type system</b>
</p>

---

Dynamic information flow control (IFC) tracks security labels at runtime and checks them before data leaves the program. This tracking is costly. MinIF is a compiler that reduces its overhead. It uses a security type system to predict statically which runtime checks always succeed, and it removes these checks together with the label tracking that no remaining check requires.

MinIF was presented at OOPSLA 2026:

> Daniel Galán Pascual, François Hublet, Srđan Krstić, Roman Fischer, Colin Pfingstl, and David Basin.
> **A Type System for Optimizing Dynamic IFC.**
> Proc. ACM Program. Lang. 10, OOPSLA2, Article 324 (2026).
> https://doi.org/10.1145/3839456

## Paper and artifact

- The artifact evaluated for the paper (version 0.3.0-ae) is archived at https://doi.org/10.5281/zenodo.21773325.
- The extended version of the paper, which includes all appendices, is archived at https://doi.org/10.5281/zenodo.21891444.

## Upcoming release

MinIF will be developed in this repository. The next release, MinIF 0.3.1, is in preparation and will be published here soon.

The artifact on Zenodo was packaged to reproduce the evaluation of the paper. With this repository, we aim to grow MinIF beyond the paper into a tool that others can use and build on, with a focus on usability and documentation.

After publication, we also identified defects in the implementation that affect the two case studies. We are correcting these defects and revising the evaluation. Preliminary measurements indicate that the overhead reductions are smaller than those reported in the paper but remain substantial. The release will include the final measurements.

## Citation

```bibtex
@article{galan_minif_2026,
  author  = {Gal{\'a}n Pascual, Daniel and Hublet, Fran{\c{c}}ois and Krsti{\'c}, Sr{\dj}an and Fischer, Roman and Pfingstl, Colin and Basin, David},
  title   = {A Type System for Optimizing Dynamic {IFC}},
  journal = {Proc. ACM Program. Lang.},
  volume  = {10},
  number  = {OOPSLA2},
  articleno = {324},
  year    = {2026},
  doi     = {10.1145/3839456}
}
```

## License

MinIF is released under the [Apache License 2.0](LICENSE).

---

<p align="center">
  <sub>Information Security Group, ETH Zurich</sub>
</p>
