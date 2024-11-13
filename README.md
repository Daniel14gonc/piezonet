# PIEZONET: Simulación de Fenómenos Físicos con PINNs

**PIEZONET** es una colección de notebooks diseñados para modelar diferentes fenómenos físicos utilizando **Redes Neuronales Informadas por Física (PINNs)**. Estos notebooks abarcan aplicaciones en transferencia de calor, dinámica de fluidos y efectos piezoeléctricos. 

Este es el código creado para el proyecto de graduación de la carrera de licenciatura en Ingeniería en Ciencias de la Computación de la Universidad del Valle de Guatemala.

---

## Estructura del Proyecto

El proyecto está organizado en carpetas según los fenómenos modelados:

### 1. **Heat**
   - **Notebook**: [heat_PINN.ipynb](./Heat/heat_PINN.ipynb)  
     **Descripción**:  
     Este notebook implementa un modelo para resolver problemas de **transferencia de calor**. Utiliza PINNs para simular la ecuación del calor en un una varilla de una dimensión.
     **Entorno de ejecución**:
        - Procesador: 11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz, 2304 MHz, 8 núcleos, 16 procesadores lógicos.
        - Memoria RAM: 32 GB.
---

### 2. **Navier-Stokes**
   - **Notebook**: [NS_PINN_geo.ipynb](./Navier-Stokes/NS_PINN_geo.ipynb)  
     **Descripción**:  
     Aquí se modelan problemas relacionados con la **dinámica de fluidos** a través de las ecuaciones de Navier-Stokes. Este notebook está diseñado para demostrar cómo las PINNs pueden abordar la simulación de un flujo en un conducto que tiene un cilindro en medio. El análisis está hecho en estado estacionario.
    **Entorno de ejecución**:
        - Google Colab: GPU Tesla T4.
        - Memoria RAM: 15 GB.
---

### 3. **Piezoelectricity**

   - **Notebook 1**: [Geometric_creation.ipynb](./Piezoelectricity/Geometric_creation.ipynb)  
     **Descripción**:  
     Este notebook genera los puntos de colocación y de frontera para una **viga en voladizo** que se modela bajo el efecto piezoeléctrico. Proporciona la base geométrica para los otros notebooks relacionados con el efecto piezoeléctrico.  
     **Entorno de ejecución**:
        - Google Colab (sin GPU Tesla T4).
        - Memoria RAM: 15 GB.

   - **Notebook 2**: [Indirect_effect_PINN.ipynb](./Piezoelectricity/Indirect_effect_PINN.ipynb)  
     **Descripción**:  
     Este notebook aborda el **efecto piezoeléctrico indirecto**, donde una estimulación eléctrica en un material genera una deformación mecánica. Está enfocado en modelar una viga en voladizo piezoeléctrica en 2D.

   - **Notebook 3**: [Direct_effect_PINN.ipynb](./Piezoelectricity/Direct_effect_PINN.ipynb)  
     **Descripción**:  
     Este notebook se enfoca en modelar el **efecto piezoeléctrico directo**, en el cual las deformaciones mecánicas en un material generan una respuesta eléctrica (voltaje). Está enfocado en modelar una viga en voladizo piezoeléctrica en 2D.

   

  - **Entorno de ejecución (para los notebooks de Direct y Indirect effect)**:
    - **Plataforma**: Google Colab (con GPU Tesla T4).
    - **Memoria RAM**: 15 GB.

---

## Con respecto al uso

El notebook de la ecuación de calor puede ser descargado y ejecutado sin ninguna configuración necesaria. Solamente, es necesario revisar si se cuenta con las librerías necesarias para ejecutarlo. Para los otros notebooks, es necesario realizar modificaciones para que puedan ser ejecutados en un entorno local o en un entorno de Google Colab.
