1. Build tensorflow from source

    1. Download correct version of bazel:
        1.1 r1.14 - `wget --no-check-certificate https://github.com/bazelbuild/bazel/releases/download/0.26.1/bazel-0.26.1-installer-linux-x86_64.sh1`
        1.2 r1.13 - `wget --no-check-certificate https://github.com/bazelbuild/bazel/releases/download/0.21.0/bazel-0.21.0-installer-linux-x86_64.s1`
    2. `chmod +x bazel-0.26.1-installer-linux-x86_64.sh`
    3. `./bazel-0.26.1-installer-linux-x86_64.sh`
    4. `git clone https://github.com/tensorflow/tensorflow.git`
    5. `cd tensorflow/`
    6. `git checkout r1.14`
    7. `./configure`
    8. `bazel build --config=opt --config=mkl --distdir ./deps //tensorflow/tools/pip_package:build_pip_package`
