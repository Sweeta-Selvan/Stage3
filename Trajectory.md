**Cell types identified at each infection stage**

* **1 dpi**

  * Ciliated cells

  * Clara cells (club cells)

  * Pulmonary alveolar type I cells (AT1)

  * Ionocytes

  * Airway goblet cells

* **2 dpi**

  * Airway goblet cells

  * Ciliated cells

  * Clara cells (club cells)

  * Pulmonary alveolar type I cells (AT1)

  * Pulmonary alveolar type II cells (AT2) — appears in your extra mapping for cluster 9

  * Ionocytes

* **3 dpi**

  * Ciliated cells

  * Ionocytes

  * Pulmonary alveolar type I cells (AT1)

  * Airway goblet cells

  * Clara cells (club cells)

  * Generic “Airway epithelial cells” (cluster annotated that way)

  * Alveolar macrophages

  2\.  The cell types identified at 1 dpi, 2 dpi, and 3 dpi correlate with COVID-19 infection because many of them share biological properties similar to **ependymal cells, neurons, cholangiocytes, myoepithelial cells, T cytotoxic cells, keratinocytes, ionocytes, luminal epithelial cells**, and other barrier/secretory/transport-active tissues that SARS-CoV-2 typically targets.

### **Ciliated cells — motile, transport-active, high ACE2 (similar to ependymal cells)**

Ciliated epithelial cells resemble **ependymal cells** in the brain because both:

* have **motile cilia**

* perform **fluid transport**

* show high **ACE2** expression

Since SARS-CoV-2 uses ACE2 to enter cells, these motile/transport-focused cells are extremely vulnerable.  
 **Upregulation** of interferon genes and **downregulation** of ciliary genes are hallmarks of infected ciliated cells.

---

### **Goblet cells — mucus-secreting cells similar to luminal epithelial cells**

Goblet cells behave like **luminal epithelial cells** in other organs:

* high secretory activity

* exposed directly to the airway lumen

* moderate ACE2 expression

They show:

* **upregulation** of inflammatory genes

* **downregulation** of normal mucus-regulation pathways.

These changes occur because the **virus** disrupts the epithelial barrier.

---

### **Clara (Club) cells — detoxifying epithelial cells similar to cholangiocytes**

Club cells share properties with **cholangiocytes** (bile duct epithelium):

* strong detox and stress-response pathways

* ability to regenerate epithelium

* sensitivity to viral stress

They react to SARS-CoV-2 by **upregulating** interferon genes and injury-response programs.

---

### **Ionocytes — rare but ACE2-high**

Ionocytes show extremely high ACE2 expression and behave similarly to **keratinocytes** in the epidermis:

* both are rare cell types

* both have specialized ion-transport roles

* both show strong **upregulation** of antiviral pathways during infection

Their role in chloride/ion transport makes them transcriptionally reactive to viral injury.

---

### **AT1 and AT2 alveolar cells — similar to myoepithelial cells and luminal epithelial cells**

AT2 cells behave somewhat like **myoepithelial** or **luminal epithelial** cells in other tissues:

* they produce surfactant (secretory function)

* they regenerate damaged epithelium

* They show both ACE2-dependent and ACE2-independent viral response.

Their infection leads to:

* **downregulation** of normal surfactant pathways

* **upregulation** of inflammatory/stress genes

This is crucial in COVID-19 lung pathology.

**6\. Macrophages at 3 dpi — immune activation similar to T cytotoxic cells**

By 3 dpi I observed **alveolar macrophages**, which correlates with:

* recruitment of immune cells  
* activation of **T cytotoxic** pathways

* clearing infected epithelial cells

These immune cells respond to viral antigens produced by infected epithelium.

3\. In  dataset, **ACE2 expression is  low, sparse, and restricted to only a few epithelial subtypes**, mainly:

* **Ionocytes** (where ACE2 is naturally high)

* A small subset of **ciliated cells**

* Rare keratinocyte-like airway cells

Because ACE2 is expressed in so few cells, it does **not increase proportionally** with infection progression (1 dpi → 2 dpi → 3 dpi).  
 This means:

* Infection spreads **even when ACE2 levels remain the same**

* Infected clusters do **not show ACE2 upregulation**

* Viral load increases, but ACE2 does **not correlate** with that increase

This pattern is well-known in SARS-CoV-2 scRNA-seq datasets:  
 **ACE2 is the entry receptor, not a dynamic infection biomarker.**

Many infected cells actually show **downregulation** of ACE2 after the virus enters (to avoid triggering interferon responses).

In contrast, viral response genes (e.g., ISGs) show:

* **Strong upregulation** in infected cells

* Consistent marking of infection trajectory

So **ACE2 does not track infection**, but **interferon-stimulated genes do**.

4\. **What ACE2 tells you**

ACE2 indicates **which cell types the virus *can* enter**, especially:

* **Ionocytes** (ACE2-high)

* A small fraction of **ciliated cells**

ACE2 expression is:

* **Low and sparse** across most airway epithelial cells

* **Not upregulated** during infection

* Sometimes **downregulated** after viral entry

This means ACE2 does **not** increase when infection worsens.

### **Why ACE2 fails as a dynamic biomarker**

* The **virus** does not induce ACE2

* Infected cells often show **ACE2 downregulation**

* Many infected clusters (e.g., Clara/club cells) have very low ACE2

So ACE2 shows **susceptibility**, but not **infection level**.

---

# **ENO2 — A marker of active viral response**

**ENO2** (Neuron-specific enolase) is not neuron-specific in scRNA-seq; it becomes highly expressed in **stressed, metabolically activated, virus-exposed epithelial cells**.

### **What ENO2 tells you**

ENO2 increases when:

* Viral replication triggers **metabolic stress**

* Interferon pathways are **upregulated**

* Airway epithelium activates glycolytic and stress programs

* Cells shift toward “keratinocyte-like” damage signatures (seen in severe infection)

In both SARS-CoV-2 studies, ENO2 is:

* **Highly expressed in infected ciliated cells**

* **Upregulated** in inflamed epithelial clusters

* A strong **dynamic biomarker** of infection progression

Unlike ACE2, ENO2 goes **up** with increasing viral burden.

5\. **Ionocyte clusters** show the highest per-cell ACE2 expression at 3 dpi (in  annotations these are clusters labeled `10`, `11` and `8`; cluster **10** is a clear example of an ACE2-high cluster).

---## **Visual / intuitive interpretation**

If I plot this in cluster violin/dotplots:
* **Violin plot (ACE2 by cluster)**: Ionocyte clusters have the **highest median and long upper tails** — meaning most ionocytes express low-to-moderate ACE2, but a subpopulation expresses very high ACE2.


Visually this means: **ACE2 signal is concentrated, not widespread** — bright islands of expression rather than a broad wave across all epithelial clusters.

