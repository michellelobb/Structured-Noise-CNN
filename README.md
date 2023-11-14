<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- ABOUT THE PROJECT -->
## About The Project

This is the code for my thesis titled "Noise in Deep Learning." The purpose of the project is to investigate the impact that total variation regularization has on structured noise in image classification problems. Structured noise is a prevalent
concern in image processing, as the noise behaves more like a wanted signal than typical random noise. 

The notebooks each correspond to one of the three tests performed on the two datasets, CIFAR-10 and Fashion MNIST. The testing was done by first creating a noise generator, then overlaying the noise over the base image. How noisy the image turned out was
dictated by the interpolation alpha factor. An $\alpha$ value of 0 means that the base image would remain unchanged, and an $\alpha$ value of 1 means only the pattern from the noise generator would be returned. After completing the noise generation, I split the
training data into five groups, with noise added to certain percentages - 0%, 25%, 50%, 75%, and 100% - of the observations. I then built a ConvNet trained on the base data to handle the classification task, and used accuracy as the performance metric.

The RGB testing showed an average accuracy increase of 3.93% for $\alpha$ = 0.1, 8.58% for $\alpha$ = 0.25, and no change for $\alpha$ = 0.5. The grayscale testing showed no improvement, due to TV regularization mathematically not handling sharp edges well.
<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ROADMAP -->
## Roadmap

- [x] Noise Generation
- [x] Proof of Concept Testing
- [ ] Medical Imaging
    - [ ] Noise Generation for Side Lobe Noise in Ultrasounds
    - [ ] Testing with the Noise Generator on Clean Images
    - [ ] Testing on Ultrasound Images

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- CONTACT -->
## Contact

Michelle Lobb - michelle.e.lobb@gmail.com

Project Link: [https://github.com/michellelobb/Structured-Noise-CNN](https://github.com/michellelobb/Structured-Noise-CNN)

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/michellelobb/Structured-Noise-CNN.svg?style=for-the-badge
[contributors-url]: https://github.com/michellelobb/Structured-Noise-CNN/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/michellelobb/Structured-Noise-CNN.svg?style=for-the-badge
[forks-url]: https://github.com/michellelobb/Structured-Noise-CNN/network/members
[stars-shield]: https://img.shields.io/github/stars/michellelobb/Structured-Noise-CNN.svg?style=for-the-badge
[stars-url]: https://github.com/michellelobb/Structured-Noise-CNN/stargazers
[issues-shield]: https://img.shields.io/github/issues/michellelobb/Structured-Noise-CNN.svg?style=for-the-badge
[issues-url]: https://github.com/michellelobb/Structured-Noise-CNN/issues
[license-shield]: https://img.shields.io/github/license/michellelobb/Structured-Noise-CNN.svg?style=for-the-badge
[license-url]: https://github.com/michellelobb/Structured-Noise-CNN/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/michelle-lobb-94a038222/
[product-screenshot]: images/screenshot.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
