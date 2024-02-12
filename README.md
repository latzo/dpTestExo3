# dpTestExo3

1. Définition des termes suivants :

   - Business Intelligence : Ensemble des technologies et pratiques visant à collecter, intégrer, analyser et présenter les informations pertinentes pour aider à la prise de décision au sein d'une entreprise
   - ETL : Extract, Transform and Load. Processus essentiel en BI qui consiste à extraire des données à partir de sources diverses, à les transformer pour les rendre cohérentes et exploitables, puis à les charger dans une destination cible (BD, entrepôt de données)
   - Table de fait : Feprésente les événements, les transactions ou les mesures quantitatives sur lesquelles les analyses et les rapports sont basés
   - Table de dimension : Contient les attributs qui permettent de qualifier, d'organiser et de filtrer les données présentes dans les tables de fait

2. Commentaire du schéma en expliquant les différents éléments constitutifs :
     -  Datasource : Il s'agit de la source des données, qui peut être située sur le réseau local de l'entreprise. Cela peut inclure des bases de données, des fichiers plats, des systèmes ERP ou d'autres systèmes internes où les données sont générées et stockées
     -  Ingestion Storage Blob : Une fois que les données sont extraites de la source, elles sont ingérées dans un stockage Blob Azure. Les blobs sont des objets de stockage de données dans le cloud Azure, offrant une grande capacité de stockage et une scalabilité élevée.
     -  Data Storage Azure Synapse : Azure Synapse (anciennement Azure SQL Data Warehouse) est une solution de stockage de données et de traitement analytique qui permet d'interroger et d'analyser de vastes ensembles de données. Il offre des fonctionnalités de traitement massivement parallèle et de requêtage SQL pour des analyses rapides et approfondies
     -  Analysis Service : Azure Analysis Services est un service d'analyse en ligne qui permet de modéliser, d'analyser et de visualiser les données stockées dans Azure Synapse et d'autres sources de données. Il offre des fonctionnalités avancées telles que la modélisation de données, la création de mesures et de dimensions, ainsi que des capacités de traitement analytique en temps réel
     -  Visualization Power BI Dashboard : Power BI est une plateforme de visualisation de données qui permet de créer des tableaux de bord interactifs, de rapports et de visualisations à partir des données stockées dans Azure Synapse et d'autres sources de données. Les utilisateurs peuvent explorer les données, créer des visualisations dynamiques et partager des insights avec d'autres membres de l'organisation
     -  Authentication Azure Active Directory : L'accès au dashboard Power BI ainsi qu'à Azure Analysis Service est protégé par authentification via Azure Active Directory (Azure AD) qui est un service d'authentification basé sur le cloud fourni par Microsoft. Il offre des fonctionnalités d'identification et de gestion des identités pour les applications cloud.
