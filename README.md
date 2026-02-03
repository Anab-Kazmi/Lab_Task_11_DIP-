# **Task 11: Morphological Operations**

**Roll Number:** 2023-SE-06

---

### **Prompt**

*"Create a Python program for LAB 11 – Morphological Operations using OpenCV. The program should allow the user to upload an image in Google Colab, automatically convert it to binary if it is grayscale, and perform the following tasks:

* Perform erosion, dilation, opening, and closing with a configurable kernel size.
* Extract boundaries using erosion.
* Fill holes using morphological reconstruction.
* Remove noise using morphological opening.
* Detect shapes (triangles, rectangles, circles, unknown) and label them on the image.
* Display all intermediate and final results in a 3x3 grid with titles.
* The code should be modular, using separate functions for each operation, handle non-binary images, and have clear visualizations with proper colormaps.
* Ensure compatibility with Google Colab file upload."*

---

## **Objective**

The objective of this task is to explore **morphological operations** in image processing. Morphological operations manipulate the structure of objects in binary or grayscale images, which is useful for:

* Noise removal
* Boundary extraction
* Hole filling
* Shape detection and labeling

This lab demonstrates both **basic operations** (erosion, dilation, opening, closing) and **advanced tasks** like **morphological reconstruction** and **shape detection**.

---

## **Methodology / Approach**

1. **Upload Image:** User uploads a grayscale or binary image using Google Colab.

2. **Binary Conversion:** Automatically convert the grayscale image to binary using thresholding.

3. **Morphological Operations:**

   * Erosion
   * Dilation
   * Opening
   * Closing
   * Noise removal using opening

4. **Boundary Extraction:** Compute boundaries by subtracting the eroded image from the original binary image.

5. **Hole Filling:** Fill holes in objects using morphological reconstruction.

6. **Shape Detection:** Detect triangles, rectangles, circles, and unknown shapes using contour approximation and label them on the image.

7. **Visualization:** Display all results in a **3×3 grid** with appropriate titles.

---

## **Results / Observations**

* **Erosion:** Shrinks foreground objects, useful to remove small noise points.
* **Dilation:** Expands objects, fills small gaps.
* **Opening:** Removes noise while preserving shape (erosion followed by dilation).
* **Closing:** Fills small holes (dilation followed by erosion).
* **Boundary Extraction:** Clearly highlights object boundaries.
* **Hole Filling:** Fills internal holes in objects effectively.
* **Noise Removed:** Morphological opening removes small isolated noise pixels.
* **Shape Detection:** Correctly identifies triangles, rectangles, circles, and labels unknown shapes.

**Observation:** Morphological operations are powerful for structural image analysis, noise reduction, and shape extraction.

---

## **Tools and Libraries Used**

* **Python 3.x**
* **OpenCV (cv2):** Image reading, thresholding, morphology, contours
* **NumPy (np):** Array manipulation, kernel creation
* **Matplotlib (plt):** Visualization in 3×3 grid
* **Google Colab:** Safe file upload and execution environment

---
