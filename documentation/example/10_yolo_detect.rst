20类识别
==============

代码
-----------
例程::

    from mpython import *
    from camera import *
    import time

    camera = CameraV831(tx=Pin.P16, rx=Pin.P15)
    camera.yolo_detect_init()
    while True:
        camera.yolo_detect.recognize()
        if camera.yolo_detect.id != None:
            print(str('category：') + str(camera.yolo_detect.category_list[camera.yolo_detect.id]))
            print(str('Confidence：') + str(camera.yolo_detect.max_score))
        time.sleep_ms(20)


mPython图形化示例
-----------
.. figure:: /_static/image/example/yolo_detect/yolo_detect.png
    :align: center
    :width: 1080