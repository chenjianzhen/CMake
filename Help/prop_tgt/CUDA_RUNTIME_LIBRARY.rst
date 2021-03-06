CUDA_RUNTIME_LIBRARY
--------------------

Select the CUDA runtime library for use by compilers targeting the CUDA language.

The allowed case insensitive values are:

.. include:: CUDA_RUNTIME_LIBRARY-VALUES.txt

Contents of ``CUDA_RUNTIME_LIBRARY`` may use
:manual:`generator expressions <cmake-generator-expressions(7)>`.

If this property is not set then CMake uses the default value
``Static`` to select the CUDA runtime library.

.. note::

  This property has effect only when the ``CUDA`` language is enabled. To
  control the CUDA runtime linking when only using the CUDA SDK with the
  ``C`` or ``C++`` language we recommend using the :module:`FindCUDAToolkit`
  module.
