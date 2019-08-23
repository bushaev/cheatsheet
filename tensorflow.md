1. Build tensorflow from source

    ```bash
    wget --no-check-certificate https://github.com/bazelbuild/bazel/releases/download/0.26.1/bazel-0.26.1-installer-linux-x86_64.sh
    chmod +x bazel-0.26.1-installer-linux-x86_64.sh
    ./bazel-0.26.1-installer-linux-x86_64.sh
    git clone https://github.com/tensorflow/tensorflow.git
    cd tensorflow/
    git checkout r1.14
    bazel shutdown```
