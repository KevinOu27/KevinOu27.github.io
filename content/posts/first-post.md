+++
title = "Diagnosing Brain Tumors with Deep Learning and Knowledge Graphs"
date = 2024-12-18T10:00:00+09:00
draft = false
+++

Applying artificial intelligence to real-world problems can be incredibly rewarding, and my recent project combining deep learning and knowledge representation for brain tumor classification has been one of the most illuminating experiences of my journey in data science. This project explored the intersection of computer vision and knowledge representation, providing not only technical challenges but also valuable insights into the potential and limitations of AI in medical applications.

![Alt text](/images/brain_tumor_project.jpeg)

**Tackling a Real-World Challenge**

The goal was ambitious: classify brain MRI images into four categories (glioma, meningioma, pituitary tumor, and no tumor) using a convolutional neural network (CNN) while linking predictions to clinical symptoms through a knowledge graph. This dual focus on accuracy and interpretability made the project especially impactful, as it bridged the gap between automated diagnosis and actionable insights for clinicians.

**Designing a Robust Deep Learning Model**

I selected the Xception architecture for the classification task, leveraging transfer learning to build a high-performing model. Data augmentation was crucial for improving generalization, applying techniques such as rotations, zooming, and brightness adjustments. Regularization methods like dropout layers, early stopping, and learning rate scheduling ensured the model didn’t overfit, resulting in a final test accuracy of 97.94%. This high performance demonstrated the effectiveness of carefully designed neural networks and highlighted the importance of structured experimentation in achieving reliable results.

**Integrating Knowledge Representation**

To make the model predictions interpretable, I integrated a static knowledge graph mapping tumor types to their associated symptoms, such as headaches and seizures for glioma or vision loss for pituitary tumors. While I initially attempted to use the Google Knowledge Graph API for dynamic symptom retrieval, its lack of medical-specific information highlighted a key limitation of general-purpose APIs in specialized domains. Falling back on static relationships derived from trusted sources like the Mayo Clinic ensured the system remained clinically relevant.

**Key Insights and Lessons Learned**

This project wasn’t without its challenges. Addressing class imbalances in the dataset, handling overfitting, and debugging feature mapping issues for explainability were all significant hurdles. However, the lessons I learned were equally valuable:
- The importance of balancing model performance and interpretability, especially in medical AI applications.
- The need for domain-specific APIs or datasets when integrating external knowledge systems.
- How regularization techniques and carefully crafted architecture can lead to efficient, reliable models.

**Broad Implications**

This project goes beyond brain tumor classification. It demonstrates how combining AI techniques—deep learning and knowledge representation—can enhance decision support systems in various domains, from healthcare to business analytics. The challenges and solutions from this experience have provided me with a stronger understanding of how to approach complex, interdisciplinary projects effectively.

Building this system wasn’t just about achieving technical milestones—it was about understanding how AI can impact people’s lives. This experience has solidified my passion for developing AI solutions that are not only accurate but also meaningful and actionable.
