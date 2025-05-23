<center>
  
---

🌳 **About o Amazon Bark** 🌳

---

Amazon Bark is a dataset composed of bark (rhytidome) images from tree species that are commercially exploited for timber purposes in the Brazilian Amazon. The dataset contains a total of 2,803 images representing 16 species. Images were collected from 10 trees per species using two devices: a CANON digital camera and an iOS iPhone 11, with resolutions of 3024 × 4032 and 4000 × 5328 pixels, respectively. The images were captured in three Forest Management Areas (FMAs), located in the municipalities of Nova Maringá, Feliz Natal, and Cotriguaçu, in the state of Mato Grosso. Botanical collections were conducted on five trees per species, with specimens prepared as herbarium vouchers and deposited at the Felisberto Camargo Herbarium (HFC) of the Federal Rural University of the Amazon. 

---
|                 Espécies                  |  n   |
|:-----------------------------------------:|------|
|Apuleia leiocarpa (Vogel) J. F. Macbr.     | 01   |
|Astronium lecointei Ducke                  | 02   |
|Bagassa guianensis Aubl.                   | 03   |
|Bowdichia nitida Spruce ex Benth.          | 04   |
|Cedrela odorata L.                         | 05   |
|Dipteryx odorata (Aubl.) Forsyth f.        | 06   |
|Erisma uncinatum Warm.                     | 07   |
|Goupia glabra Aubl.                        | 08   |
|Hymenolobium petraeum Ducke                | 09   |
|Mezilaurus itauba (Meisn.) Taub. ex Mez    | 10   |
|Parkia pendula (Willd.) Benth. ex Walp.    | 11   |
|Protium acrense Daly                       | 12   |
|Qualea paraensis Ducke                     | 13   |
|Simarouba amara Aubl.                      | 14   |
|Trattinnickia burserifolia Mart.           | 15   |
|Vatairea sericea (Ducke) Ducke             | 16   |

</center>

---
Data Partitioning

A stratified split was applied, assigning 80% and 20% of the images to training and testing sets, respectively. This partitioning preserved class proportions (80% and 20%) within each set. The splitfolders Python library was used to perform and save these partitions automatically to the drive. Subsequently, 50 patches of 256 × 256 pixels were extracted from each image, resulting in 111,850 patches for training and 28,300 for testing—a total of 140,150 patches derived from the 2,803 original images.

Feature Extraction

- Variations of the Local Binary Pattern (LBP) operator were employed, including Uniform, Rotation-Invariant, and Non-Rotation-Invariant patterns.

- Four pre-trained Convolutional Neural Networks (CNNs) were used as feature extractors, loaded with ImageNet weights: ResNet50, VGG16, InceptionV3, and MobileNetV2.

Classification

- Four machine learning algorithms were applied: Support Vector Machines (SVM), Artificial Neural Networks (ANN), Random Forest (RF), and Linear Discriminant Analysis (LDA).
---
