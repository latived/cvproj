# cvproj
computer vision project code

project info
---

Relatório:
- Descritivo das etapas e referências utilizadas na execução da etapa.
- Descrição das dificuldades encontradas e soluções testadas (mesmo as que não funcionaram).
- Passo-a-passo detalhado de como repetir a etapa.
- Descrição de todas as ferramentas utilizadas (APIs, SDKs, IDEs) e especificação das versões de todas as ferramentas e/ou plataformas.
- Tudas essas informações devem ser "upadas" para um repositório git.

Apresentação:
- Apresentação do relatório em slides.
- Apresentação do código funcionando.

Repositório:
- Atualização de um repositório git onde a solução possa ser encontrada e reproduzida por alunos de semestres futuros.

---

Timeline
---

Before 13/09/18

- Started to search for android tutorials and android + opencv tutorials.
- Successfully builded, installed and tested 'face-detection' sample project.
- After changed Android and OpenCV-android-sdk folders, I couldn't build the project again. Gave up for a period.

13 Set 18

- This repo is created.
- Started (again) to search for android tutorials and android + opencv tutorials.
- First milestone is setted.
- Build first android app (basic, not uploaded here; see android dev guide).

15 Set 18

- Reading about activities and its lifecycle.
- Trying install and test some sample app.

16 Set 18

- Successfully builded, installed and tested 'tutorial-2-mixedprocessing' sample project:
	1. In build.gradle from project add 'google()' in 'repositories' block (both of them).
	2. In build.gradle files from both modules modify 'compileSdkVersion' and 'targetSdkVersion' to be the same.
	4. Make sure 'local.properties' has the right path to 'ndk.dir' and 'sdk.dir' (usually 'Android/Sdk/ndk-bundle' and 'Android/Sdk').
	5. Right-click in 'openCVTutorial2MixedProcesing' and select 'Link C++ Project with Gradle'.
	6. Select 'ndk-build' in 'Build System'.
	7. Select path for 'Android.mk' (usually is src/main/jni/Android.mk).
	8. Open 'Android.mk' and modify (last 'include', for example) path to 'OpenCV.mk' (look inside 'path-to-OpenCV-android-sdk/sdk/native/jni').
	9. Open 'Application.mk' (same folder as 'Android.mk') and modify APP\_ABI to 'all' or your device arch.
	10. Open AndroidManifest.xml from 'openCVTutorial2MixedProcessing' and delete 'android:theme'.
	11. Install OpenCV Manager of the same arch as your device (see inside 'path-to-OpenCV-android-sdk/apk').
	12. Build project and install apk (you can do this from Android Studio directly).
	13. If an error appears on the device screen, you must give it permission to use the camera: go to its 'App info' and in 'Permissions' turn on 'Camera'.


Tutorials
---

- https://medium.com/@sukritipaul005/a-beginners-guide-to-installing-opencv-android-in-android-studio-ea46a7b4f2d3 (ignore step 6; unecessary)
- https://android.jlelse.eu/a-beginners-guide-to-setting-up-opencv-android-library-on-android-studio-19794e220f3c (ignore step 6 too)
- https://developer.android.com/guide/?hl=pt-br
