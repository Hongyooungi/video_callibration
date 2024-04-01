# video_callibration
This program alleviates camera distortion through camera calibration.

- 카메라 캘리브레이션-

1. 카메라를 이용해서 chessBoard를 촬영 후 my_chessboard.avi 파일을 만든다
2. my_chessboard.avi 를 camera_calibration.py 를 이용해서 캘리브레이션 수행

-> 수행 결과:
The number of selected images = 26
RMS error = 1.1604022898278548
Camera matrix (K) = 
[[1.01212241e+03 0.00000000e+00 9.54081522e+02]
 [0.00000000e+00 1.01205120e+03 5.41382436e+02]
 [0.00000000e+00 0.00000000e+00 1.00000000e+00]]
 Distortion coefficient (k1, k2, p1, p2, k3, ...) = [ 0.00020659  0.02590867 -0.00105908  0.00307626 -0.02384998]


 ![chessboard01](https://github.com/Hongyooungi/video_callibration/assets/127743990/7676d619-da5d-49e8-b64d-c1ac6cc71490)



 

 - 카메라 렌즈 왜곡 보정 기능 -

1. 위의 캘리브레이션을 통해 얻은 값들로 distortion_correction.py를 통해 렌즈 왜곡 보정 수행


![chessboard02](https://github.com/Hongyooungi/video_callibration/assets/127743990/6ff2e201-f228-4240-beea-eeace4bcbad6)


- 본 동영상은 갤럭시 카메라의 광각 모드를 사용하여 촬영을 하였다.
고프로와는 달리 카메라의 렌즈 왜곡 현상이 두드러지게 나타나지 않아서 카메라 왜곡 보정이 잘 되었는지 육안으로 판단하기 어렵다.
따라서, 왜곡이 심한 고프로와 같은 카메라로 테스트를 해보아야 할 것 같다. 
 
