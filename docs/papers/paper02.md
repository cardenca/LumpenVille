# Computation of faulty IV-curves based on a distributed solar cell algorithm

 September 20, 2022

---

*Authors: Carlos Cárdenas-Bravo, Denys Dutykh, and Sylvain Lespinats Conference: 8th World Conference on Photovoltaic Energy Conversion, 26 – 30 September 2022, Milan, Italy. Corresponding author: carlos.cardenas@cea.fr

---



Several explanations have been proposed in the literature to represent defects in solar modules. However, despite the nature of the failure, the available data indicates that defects in a solar module can be modeled by modifying the internal parameters of the solar cells that compose the module. Consequently, having software capable of generating IV curves based on a distributed solar cell model represents an advantage for acquiring in-deep knowledge about the failure phenomena in solar modules. In addition, having access to such algorithms opens the possibility of creating new approaches, such as the generation of a thermal image based on the internal parameters of a solar module cell and environmental data (plane of array irradiance matrix, ambient temperature, and wind speed).

There are different ways to calculate the electrical behavior of a solar module at different levels. One example of this is the well-known PVlib open-source library, which is capable of calculating atmospheric variables, as well as DC and AC electrical variables of large PV systems. This library offers the possibility of modifying the irradiance on the plane and the cell temperature assuming a uniform distribution. However, lacks the option of introducing mismatches in a solar array, which is a limiting factor when analyzing faulty scenarios. Therefore, specialized software is required to solve these cases.

Another well-known and widely software used is PVmismatch. This software, as well as PVlib, is able to calculate IV curves at different levels of irradiation and cell temperatures for the distinct sections of a solar plant, i.e., solar cell, solar module, solar string, and solar system level. However, the advantage of PVmismatch is that the user can calculate IV curves when having different irradiances or cell temperatures at the cell level (for a solar module) or module level (for a solar string or solar system). This feature provides a degree of flexibility when studying the faults present in the solar system. Despite these advantages, PVmismatch is not capable of calculating atmospheric variables, or the AC generation of a photovoltaic system. Therefore, a complete analysis should be performed mixing both PVlib and PVmismatch libraries.

This work proposes a novel calculus method that goes deeper into the nature of photovoltaic technology. For this purpose, a distributed solar cell model is used to calculate the IV curves of a solar module. The main advance of this approach is that the user can set the topology of the solar module, as well as each parameter of the solar cells that compose it. Also, the proposed calculus method offers the possibility of modifying the protection system model, adding another degree of freedom to the original problem. Finally, similarly to PVmismatch, the proposed method is able to calculate IV curves given the irradiance and cell temperature of each solar cell. 
