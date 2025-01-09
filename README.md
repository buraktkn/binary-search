# Binary Search Tree (BST)

## Problem
Dizi: **[7, 5, 1, 8, 3, 6, 0, 9, 4, 2]**

---

## Binary Search Tree Aşamaları

### 1. Root Belirleme
İlk eleman **7**, ağacın **root** düğümü olarak seçilir.  
**Root: 7**

---

### 2. Elemanları Ağaca Ekleme
Elemanlar sırasıyla ağaca yerleştirilir:

- **5**: 5, 7'den küçük olduğu için **7'nin soluna** eklenir.  
  **Root: 7**  
  Sol: 5  

- **1**: 1, 7'den küçük ve 5'ten de küçük olduğu için **5'in soluna** eklenir.  
  **Root: 7**  
  Sol: 5 → Sol: 1  

- **8**: 8, 7'den büyük olduğu için **7'nin sağına** eklenir.  
  **Root: 7**  
  Sol: 5 → Sol: 1  
  Sağ: 8  

- **3**: 3, 7'den küçük, 5'ten küçük ancak 1'den büyük olduğu için **1'in sağına** eklenir.  
  **Root: 7**  
  Sol: 5 → Sol: 1 → Sağ: 3  
  Sağ: 8  

- **6**: 6, 7'den küçük, 5'ten büyük olduğu için **5'in sağına** eklenir.  
  **Root: 7**  
  Sol: 5 → Sol: 1 → Sağ: 3  
           → Sağ: 6  
  Sağ: 8  

- **0**: 0, 7'den küçük, 5'ten küçük ve 1'den de küçük olduğu için **1'in soluna** eklenir.  
  **Root: 7**  
  Sol: 5 → Sol: 1 → Sol: 0 → Sağ: 3  
           → Sağ: 6  
  Sağ: 8  

- **9**: 9, 7'den büyük ve 8'den de büyük olduğu için **8'in sağına** eklenir.  
  **Root: 7**  
  Sol: 5 → Sol: 1 → Sol: 0 → Sağ: 3  
           → Sağ: 6  
  Sağ: 8 → Sağ: 9  

- **4**: 4, 7'den küçük, 5'ten küçük, 1'den büyük ve 3'ten büyük olduğu için **3'ün sağına** eklenir.  
  **Root: 7**  
  Sol: 5 → Sol: 1 → Sol: 0 → Sağ: 3 → Sağ: 4  
           → Sağ: 6  
  Sağ: 8 → Sağ: 9  

- **2**: 2, 7'den küçük, 5'ten küçük, 1'den büyük ve 3'ten küçük olduğu için **3'ün soluna** eklenir.  
  **Root: 7**  
  Sol: 5 → Sol: 1 → Sol: 0 → Sağ: 3 → Sol: 2 → Sağ: 4  
           → Sağ: 6  
  Sağ: 8 → Sağ: 9  

---

## Sonuç
Ağacın son hali:


         7
       /   \
      5     8
     / \      \
    1   6      9
   / \
  0   3
     / \
    2   4
