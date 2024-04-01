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


 

 - 카메라 렌즈 왜곡 보정 기능 -

1. 위의 캘리브레이션을 통해 얻은 값들로 distortion_correction.py를 통해 렌즈 왜곡 보정 수행

 
