# The Annotated Triple Product Property Matrix Multiplication Algorithm by [Murage Kibicho](https://x.com/murage_kibicho)
<p>Python guide to the obscure <strong>Triple Product Property (TPP)</strong> approach to the elusive O(n<sup>2</sup>) matrix multiplication problem.</p>

Let me know if you spot a mistake via [Twitter](https://x.com/murage_kibicho) or <a href="mailto:murage@kibicho">Email</a> (I'm also searching for a job).
### Quick Summary
We follow (Cohn & Umans, 2003) thesis in Python and observe:
1. We can embed our matrices into a group algebra.
2. Implicitly perform the matmul via convolutions within the group algebra.
3. Easily read the matrix product’s results from the group algebra.

<div align="center">
<img src="https://github.com/MurageKibicho/The-Annotated-Triple-Product-Property-Matrix-Multiplication-Algorithm/blob/main/Promo/DuaLipa.png?raw=true:" alt="Dua Lipa alongside TPP paper" width=400>
</div>

# Getting Started

### For the shape rotators:
You can follow the annotated Google Colab notebook, or `git clone` the repo and open the jupyter notebook.

### For the wordcels:
Here's a super-friendly [Substack article](https://leetarxiv.substack.com/p/triple-product-property-matrix-multiplication).

### Extended Summary
I'm going to show you how to perform linear algebra without matrices.
Microsoft and Caltech researchers (Cohn & Umans, 2003) found an FFT-style matmul algo but it's a theoretical computer science artifact.

 It's built on **four observations**:
1. Wedderburn's theorem tells us there's a structure-preserving map between the product of square matrices and the group algebra of a finite group.
<div align="center">
  <img src="https://github.com/MurageKibicho/The-Annotated-Triple-Product-Property-Matrix-Multiplication-Algorithm/blob/main/Promo/Wedderburn.png?raw=true"
       alt="Dua Lipa alongside TPP paper"
       width="600">
</div>

2. This map is a Discrete Fourier Transform.
3. Every Discrete Fourier Transform (DFT) admits a Fast Fourier Transform (FFT).
4. So there might exist an FFT-style algorithm for sub-quadratic (not even sub-cubic lol!) matrix multiplications.


This guide is best followed (in a separate tab) alongside this [LeetArxiv article](https://leetarxiv.substack.com/p/triple-product-property-matrix-multiplication). You'll see the references and coding steps.





---

###### Trump defunded my math PhD and my realtor day job contract ends on 10th July.

If you’re hiring please reach out via email: murage@kibicho.com. If not, please consider supporting my [Substack](https://leetarxiv.substack.com/p/triple-product-property-matrix-multiplication).

