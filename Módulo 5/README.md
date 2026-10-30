# Módulo 5: Dinámica de Sistemas

## Planteo del Problema: Plaga y Control Biológico en un Viñedo Mendocino
Para este trabajo se utilizó el modelo predador–presa de la cátedra, interpretado como la interacción entre la **polilla de la vid** (plaga, la presa) y su **enemigo natural** (el depredador) en un viñedo de Mendoza. Las dos poblaciones forman un sistema realimentado: cuando abunda la plaga, el enemigo natural se multiplica; al crecer el enemigo natural, la plaga disminuye; y al escasear la plaga, el enemigo natural también cae.

El objetivo fue evaluar en Vensim PLE qué ocurre si el productor combate la plaga con un **insecticida no selectivo**, que elimina tanto a la polilla como a su enemigo natural. El modelo se simuló durante 12 temporadas bajo dos escenarios:

1. **Escenario Inicial (sin intervención):** El modelo original muestra oscilaciones sostenidas y desfasadas de ambas poblaciones, con un ciclo de aproximadamente 6 temporadas alrededor del equilibrio (100 ; 28,6).
2. **Escenario de Perturbación (Función STEP):** Se agregó la variable `mortalidad por insecticida = STEP(0.3, 4)`, que desde la temporada 4 elimina un 30% adicional de ambas poblaciones por temporada.

### Conclusión Técnica
El insecticida resultó **contraproducente**. Al eliminar al enemigo natural, la plaga pierde su control biológico: su pico pasa de unas 180 a unas 300 unidades (+65%), su equilibrio sube de 100 a 130 (+30%) y las oscilaciones se vuelven más amplias y violentas. Es el llamado *principio de Volterra*: una mortalidad que afecta por igual a ambas especies termina favoreciendo a la presa. Por eso se recomiendan estrategias de control que cuiden al enemigo natural, como insecticidas selectivos o control biológico, junto con el monitoreo continuo de ambas poblaciones.

## 📥 Descargas
Los archivos del proyecto, incluyendo el informe técnico y el modelo ejecutable de Vensim, pueden descargarse directamente mediante los siguientes atajos:

[Descarga aquí el Informe Técnico en PDF](M5%20-%20TyHMII%202026.pdf)  
[Descarga aquí el Modelo de Vensim (.mdl)](Predator-Prey_insecticida.mdl)
