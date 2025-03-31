Table 1: **The classification accuracy of ViT-B-16 on ImageNet variants and cross-domain dataset.** The experimental results show that the BITTA model also demonstrates good compatibility on these different datasets.

|Method|ImageNet|ImageNet-A|ImageNet-R|ImageNet-S|ImageNet-V2|Mean|
|-|-|-|-|-|-|-|
|TPT|68.98|54.77|77.06|47.94|63.45|62.44
|TPT+BITTA|70.31|55.78|78.03|48.93|64.77|63.56
|TPS|70.10|60.80|80.28|49.59|64.83|65.12
|TPS+BITTA|72.37|62.90|81.41|50.45|65.79|66.58

|Method|Flower102|DTD|Pets|Cars|UCF101|CalTech101|Food101|SUN397|Aircraft|EuroSAT|Mean|
|-|-|-|-|-|-|-|-|-|-|-|-|
|TPT|68.98|47.75|87.79|66.87|68.04|94.16|84.67|65.50|24.78|42.44|65.10
|TPT+BITTA|70.56|48.99|87.33|67.13|68.47|94.85|86.50|66.47|26.08|44.44|66.09
|TPS|71.28|50.45|87.41|69.04|70.75|95.13|85.18|68.45|26.30|43.80|66.78
|TPS+BITTA|72.34|51.68|88.69|69.13|71.61|95.47|86.44|72.82|25.67|46.68|68.05


Table 2: **Comparision with TDA on ImageNet-C using ViT-B-16.** The experimental results show that the performance of TDA is inferior to that of BAT+BITTA. However, given the outstanding efficiency of TDA, we believe that combining the training-free strategy of TDA with the over-fitting prevention concept of BITTA will be a very valuable exploration direction in the future.

|Method|Gaussian|Shot|Impulse|Defocus|Glass|Motion|Zoom|Snow|Frost|Fog|Brightness|Constrast|Elastic|Pixelate|JPEG|Mean|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
|TDA|9.50|10.26|10.82|24.24|14.74|24.40|25.04|35.18|32.96|38.76|56.30|16.46|15.06|39.36|35.36|25.90
|BAT+BITTA|22.46|24.10|22.44|28.00|23.94|31.88|29.30|36.92|32.22|41.86|55.88|26.42|22.68|40.38|39.68|31.88


Table 3: **Comparision with MEMO and BITTA on ImageNet-C using ViT.** As can be seen, BITTA is better than marginal entropy proposed by MEMO.
|Method|Gaussian|Shot|Impulse|Defocus|Glass|Motion|Zoom|Snow|Frost|Fog|Brightness|Constrast|Elastic|Pixelate|JPEG|Mean|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
|MEMO|39.58|37.13|39.42|31.85|25.37|40.55|34.86|26.88|33.21|53.26|65.87|55.74|35.63|55.25|58.76|42.22
|MEMO+BITTA|40.69|37.74|40.83|32.97|26.63|41.49|35.86|28.69|34.21|54.93|67.84|56.21|36.74|56.85|59.47|43.41

Table 4: **The performance fluctuation of different methods.** it can be clearly seen that almost all methods will experience performance fluctuations under different noise conditions. Therefore, this phenomenon does not mean that the method we proposed lacks generalization ability.
|DPE vs TPT on CIFAR-10-C|TPT vs CLIP on CIFAR-100-C|BAT vs DPE on ImageNet-C|
|-|-|-|
|Gaussian,Shot,Impluse|Gaussian,Shot,Motion|Frost,Brightness,Contrast|
|-5.13%,-6.25%,-0.95%|-2.36%,-2.41%,-0.51%|-1.76%,-0.16%,-1.56%|
