************
Introduction
************
Ncpol2sdpa is a tool to convert a polynomial optimization problem of either commutative or noncommutative variables to a sparse semidefinite programming (SDP) problem that can be processed by the `SDPA <http://sdpa.sourceforge.net/>`_ family of solvers, `MOSEK <http://www.mosek.com/>`_, or further processed by `PICOS <http://picos.zib.de/>`_ to solve the problem by `CVXOPT <http://cvxopt.org/>`_ . The optimization problem can be unconstrained or constrained by equalities and inequalities.

The objective is to be able to solve very large scale optimization problems. Example applications include:

- Ground-state energy problems: bosonic and fermionic systems, Pauli spin 
  operators.
- Maximum quantum violation of Bell inequalities.
- Nieto-Silleras-type hierarchy for quantifying randomness.
- Moroder-type hierarchy to enable PPT-style and other additional constraints.

The implementation has an intuitive syntax for entering problems and it scales for a larger number of noncommutative variables using a sparse representation of the SDP problem. Further details are found in the following paper:

Wittek, P. (2014). `Ncpol2sdpa -- Sparse Semidefinite Programming Relaxations for Polynomial Optimization Problems of Noncommuting Variables <http://arxiv.org/abs/1308.6029>`_. To Appear in ACM Transactions on Mathematical Software.

Copyright and License
=====================
Copyright © 2012-2014 P. Wittek

Ncpol2sdpa is free software; you can redistribute it and/or modify it under the terms of the `GNU General Public License <http://www.gnu.org/licenses/gpl-3.0.html>`_ as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.

Ncpol2sdpa is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the `GNU General Public License <http://www.gnu.org/licenses/gpl-3.0.html>`_ for more details. 


Acknowledgment
==============
This work is supported by the European Commission Seventh Framework Programme under Grant Agreement Number FP7-601138 `PERICLES <http://pericles-project.eu/>`_, by the `Red Espanola de Supercomputacion <http://www.bsc.es/RES>`_ grants number FI-2013-1-0008 and  FI-2013-3-0004, and by the `Swedish National Infrastructure for Computing <http://www.snic.se/>`_ project number SNIC 2014/2-7.