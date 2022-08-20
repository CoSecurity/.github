# CoSecurity
Solução pensada para aliar segurança e inteligência a fim de tornar sua vizinhança mais segura.

Nossa premissa é a segurança colaborativa por meio da presença e gravação em nuvem, buscando inibir ações criminosas nas ruas do seu bairro e, caso aconteça, oferecendo mecanismos de ação rápida para auxiliar na resolução ágil e segura.

Acreditamos que as ruas do seu bairro pertencem a você e às pessoas bem intencionadas. Não temos que conviver com o medo, mas sim com a certeza de dias melhores. Acreditamos que devemos ter o direito de viver com segurança e compartilhar momentos tranquilos.

## Ciência de dados
Atuamos fortemente utilizando tecnicas de visão computacional e analise com series temporais, tento uma plataforma de ingestão de dados alocada na Amazon Web Services (AWS). Entre nossas tecnologias podemos destacar o uso de Tensorflow, PyTorch e OpenCV.

Nossos modelos são capazes de efetuar reconhecimento de pessoas, veiculos e objetos no geral treinados para reconhecer e determinar padrões das ruas de São Paulo. Atualmente temos modelos de detecção de anomalias de pessoas e veiculos que são capazes de determinar áreas e direção incomuns levantando em consideração o fluxo da via.

Todos os nossos modelos estão escalados por meio do AWS SageMaker efetuado interações por meio de gerações de eventos e carga de imagens via AWS S3.

Abaixo segue uma representação da nossa arquitetura do início da ingestão da imagens até as etapas de treinamento e previsão dos modelos:
![cosecurity-pipeline drawio](https://user-images.githubusercontent.com/29183537/185762400-981ab1a7-1d62-4870-9474-c5121e8d7dbb.png)

