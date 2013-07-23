#! /home/erol/android-sdks/tools/monkeyrunner
'''
Created on Jan 3, 2013

@author: erol
'''
from com.android.monkeyrunner import MonkeyRunner, MonkeyDevice


def lockDevice(device):
    return device.press("POWER", MonkeyDevice.DOWN_AND_UP)


def unlockDevice(device):
    device.wake()
    device.drag((979, 369), (1150, 380), 1.0, 120)

def main():
    device = MonkeyRunner.waitForConnection()
    if device:
        lockDevice(device)
        MonkeyRunner.sleep(5.0)
        unlockDevice(device)

if __name__ == '__main__':
    main()
