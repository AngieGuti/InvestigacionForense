# Reglas de Comportamiento y Git
* Nunca incluyas la etiqueta `Co-Authored-By` ni atribuyas commits a IA.
* Utiliza estrictamente el usuario y correo configurados en el entorno local de Git.
* Realiza commits atómicos usando Conventional Commits (feat:, fix:, docs:, chore:).
* Nunca rastrees archivos binarios ni auxiliares (*.pdf, *.aux, *.bbl, *.bcf, *.log, *.out).

# Compilación LaTeX (Docker)
* Los comandos deben ejecutarse con `-w /workspace/docs`:
  1. docker exec -w /workspace/docs forense_latex_compiler pdflatex -interaction=nonstopmode IntegraciondeIAenAnalisisForenseDigital.tex
  2. docker exec -w /workspace/docs forense_latex_compiler biber IntegraciondeIAenAnalisisForenseDigital
  3. docker exec -w /workspace/docs forense_latex_compiler pdflatex -interaction=nonstopmode IntegraciondeIAenAnalisisForenseDigital.tex
  4. docker exec -w /workspace/docs forense_latex_compiler pdflatex -interaction=nonstopmode IntegraciondeIAenAnalisisForenseDigital.tex

# Directrices de Contenido
* Alcance temático: Triaje automatizado, detección de deepfakes e IA explicable (XAI).
* Enfoque crítico: Evaluar técnica y jurídicamente las limitaciones, sesgos, sobreajuste y riesgos de caja negra frente a la admisibilidad legal.
