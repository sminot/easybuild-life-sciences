---
title: foss-2021b
date: 2020-08-01
layout: single
permalink: /toolchains/foss-2021b/
toc: true
toc_label: "On This Page"
sidebar:
  nav: "docs"
---

## foss-2021b
 FOSS - Free Open Source Software. GNU Compiler Collection (GCC) based compiler toolchain, including
 OpenMPI for MPI support, OpenBLAS (BLAS and LAPACK support), FFTW and ScaLAPACK.

 New to the 2021b toolchain is support for FlexiBLAS. There are so many linear algebra libraries that a new library needed to
be created. FlexiBLAS is not really a library but a wrapper to BLAS and LAPACK. The author has a nice video introduction and has done much work clean up the calling interfaces for BLAS and LAPACK. You can code to one standard and swap dynamicly without re-compiling.

### Package List
 * [GCCcore-11.2.0](https://gcc.gnu.org/)The GNU Compiler Collection includes front ends for
 C, C++, Objective-C, Fortran, Java, and Ada, as well as libraries for these languages (libstdc++, libgcj,...).
 * [binutils-2.37](http://directory.fsf.org/project/binutils/) binutils: GNU binary utilities
 * [GCC-11.2.0](http://gcc.gnu.org/) The GNU Compiler Collection.
 ** [numactl-2.0.13](http://oss.sgi.com/projects/libnuma/) The numactl program allows you to run your
   application program on specific cpus and memory nodes.
 It does this by supplying a NUMA memory policy to the operating system before running your program.
 The libnuma library provides convenient ways for you to add NUMA memory policies into your own program.
 ** [hwloc-2.2.0](http://www.open-mpi.org/projects/hwloc/) The Portable Hardware Locality (hwloc) software package provides a portable abstraction
 (across OS, versions, architectures, ...) of the hierarchical topology of modern architectures, including
 NUMA memory nodes, sockets, shared caches, cores and simultaneous multithreading. It also gathers various
 system attributes such as cache and memory information as well as the locality of I/O devices such as
 network interfaces, InfiniBand HCAs or GPUs. It primarily aims at helping applications with gathering
 information about modern computing hardware so as to exploit it accordingly and efficiently.
 ** [PMIx-3.1.5](https://pmix.org/) Process Management for Exascale Environments
PMI Exascale (PMIx) represents an attempt to
provide an extended version of the PMI standard specifically designed
to support clusters up to and including exascale sizes.
 * [OpenMPI-4.1.1](http://www.open-mpi.org/) The Open MPI Project is an open source MPI-2 implementation.
 * [FlexiBLAS-3.0.4](https://gitlab.mpi-magdeburg.mpg.de/software/flexiblas-release)FlexiBLAS is a wrapper library that enables the exchange of the BLAS and LAPACK implementation
used by a program without recompiling or relinking it.
 * [OpenBLAS-0.3.12](http://xianyi.github.com/OpenBLAS/) OpenBLAS is an optimized BLAS library based on GotoBLAS2 1.13 BSD version.
 including OpenMPI for MPI support.
 * [FFTW-3.3.10](http://www.fftw.org) FFTW is a C subroutine library for computing the discrete Fourier transform (DFT)
 in one or more dimensions, of arbitrary input size, and of both real and complex data.
 * [ScaLAPACK-2.1.0](http://www.netlib.org/scalapack/) The ScaLAPACK (or Scalable LAPACK) library includes a subset of LAPACK routines redesigned for distributed memory MIMD parallel computers.
 * [foss-2021b](https://raw.githubusercontent.com/easybuilders/easybuild-easyconfigs/master/easybuild/easyconfigs/f/foss/foss-2021b.eb)

