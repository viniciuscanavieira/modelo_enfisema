**DetectAI: Sistema de Detecção de Enfisema Pulmonar em Raio-X**  

Utilizando redes neurais profundas, este sistema identifica enfisema pulmonar em imagens radiográficas com alta precisão. Desenvolvido para auxiliar profissionais de saúde, o modelo foi treinado em um dataset diversificado e balanceado, garantindo robustez em diferentes cenários clínicos.  

📁 **Base de Dados**  
O treinamento utilizou o **dataset NIH Chest X-rays**, que contém imagens rotuladas para enfisema e outras condições pulmonares:  

🔗 **Acessar Dataset**: [NIH Chest X-ray Dataset](https://www.nih.gov/news-events/news-releases/nih-clinical-center-provides-one-largest-publicly-available-chest-x-ray-datasets-scientific-community)  

**Detalhes do Conjunto de Dados**:  
- Imagens de treinamento: ~112.120 (com subconjunto específico para enfisema)  
- Imagens de validação: ~14.000  
- Imagens de teste: ~5.000  
- **Rótulos**: Marcadores binários (presença/ausência de enfisema)  

**Destaque Visual**:  
O sistema inclui um módulo de interpretabilidade com **Grad-CAM** para destacar regiões suspeitas na imagem, facilitando a análise médica.  

**Técnicas Avançadas**:  
- Pré-processamento com normalização e aumento de dados (data augmentation)  
- Modelo baseado em **CNN (EfficientNet ou ResNet)** adaptado para enfisema  
- Métricas de avaliação: AUC-ROC, sensibilidade e especificidade balanceadas  

🔍 **Aplicação**:  
- Triagem automatizada em hospitais  
- Auxílio no diagnóstico precoce de doenças pulmonares crônicas  
- Integração com sistemas PACS (Picture Archiving and Communication System)  

*Obs.: O modelo foi validado em dados independentes, mas deve ser usado como ferramenta de apoio, não substituindo avaliação médica.*  

---  
**Próximos Passos**:  
1. Adaptar o código do Colab para carregar o dataset NIH.  
2. Implementar o Grad-CAM para visualização das áreas afetadas.  
3. Ajustar hiperparâmetros para otimizar a detecção de enfisema.  
