# Secondary Neutrino Flux from UHECR Propagation

A CRPropa3 tutorial notebook simulating cosmogenic (GZK) neutrino production from ultra-high-energy cosmic ray (UHECR) propagation, with comparison to IceCube observations.

**Status:** Submitted as [Pull Request #557](https://github.com/CRPropa/CRPropa3/pull/557) to the official [CRPropa/CRPropa3](https://github.com/CRPropa/CRPropa3) repository.

## Overview

Ultra-high-energy protons above ~50 EeV interact with cosmic microwave background (CMB) photons via the GZK process, producing pions that decay into secondary neutrinos. This notebook simulates that full chain using [CRPropa3](https://crpropa.github.io/CRPropa3/), the standard open-source framework for UHECR propagation.

## What's Included

- A 1D cosmological simulation of proton propagation from z=0 to z=3
- Secondary neutrino tracking via `PhotoPionProduction` on CMB and EBL photon fields
- Computation of the E² neutrino energy spectrum, compared against the IceCube diffuse flux measurement and cosmogenic upper limit
- A comparison of hard (α=−1) vs soft (α=−2) source injection spectra and their effect on the neutrino yield
- Full markdown explanations for every cell, written for the official CRPropa3 documentation

## Notebook

[`secondary_neutrino_flux.ipynb`](doc/pages/example_notebooks/secondary_neutrinos/secondary_neutrino_flux.ipynb)

Runs end-to-end in Google Colab (installs CRPropa3 from source automatically).

## Physics Motivation

Cosmogenic neutrinos are a guaranteed by-product of UHECR propagation and a key target for IceCube and KM3NeT/ARCA. This notebook extends the existing `secondaries/neutrinos.ipynb` example in CRPropa3 by adding an IceCube flux comparison and a spectral index study — directly relevant to multimessenger astroparticle physics.

## References

- Greisen (1966), *PRL* 16, 748
- Zatsepin & Kuzmin (1966), *JETP Lett.* 4, 78
- Gilmore et al. (2012), *MNRAS* 422, 3189
- Aartsen et al. / IceCube (2020), *PhRvL* 125, 121104
- Alves Batista et al. (2022), *JCAP* 09, 035 — [CRPropa3 paper](https://arxiv.org/abs/2208.00107)
