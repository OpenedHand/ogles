INCLUDES = @GCC_FLAGS@ @VINCENT_CFLAGS@ -I$(top_srcdir)/include -I$(top_srcdir)/include/GLES -I$(top_srcdir)/src/linux-x11 -I$(top_srcdir)/src/codegen

lib_LTLIBRARIES = libvincent.la

libvincent_la_LIBADD  = @VINCENT_LIBS@ 
libvincent_la_LDFLAGS = @VINCENT_LT_LDFLAGS@
libvincent_la_CFLAGS = -DHAVE_X11_EXTENSIONS_XSHM_H
libvincent_la_SOURCES =  \
      Arrays.h \
      Buffer.h \
      Color.h \
      Config.cpp \
      Config.h \
      Context.cpp \
      Context.h \
      ContextBuffer.cpp \
      ContextFloat.cpp \
      ContextLight.cpp \
      ContextLines.cpp \
      ContextMaterial.cpp \
      ContextMatrix.cpp \
      ContextMesh.cpp \
      ContextPoints.cpp \
      ContextRaster.cpp \
      ContextRender.cpp \
      ContextTexture.cpp \
      ContextTriangles.cpp \
      ContextViewport.cpp \
      Display.cpp \
      Display.h \
      FractionalColor.h \
      Light.cpp \
      Light.h \
      LineClipper.inc \
      Material.cpp \
      Material.h \
      MatrixStack.cpp \
      MatrixStack.h \
      OGLES.h \
      Rasterizer.cpp \
      Rasterizer.h \
      RasterizerState.cpp \
      RasterizerState.h \
      RasterizerTriangles.cpp \
      RasterizerTriangles.inc \
      Texture.cpp \
      Texture.h \
      TriangleClipper.inc \
      TriangleClipperHigh.inc \
      TriangleClipperLow.inc \
      Types.h \
      Utils.cpp \
      Utils.h \
      fixed.cpp \
      fixed.h \
      gl.cpp \
      gl_sin.h \
      linalg.cpp \
      linalg.h \
      arm/CodeGenerator.cpp \
      arm/CodeGenerator.h \
      arm/FunctionCache.cpp \
      arm/FunctionCache.h \
      arm/GenFragment.cpp \
      arm/GenLline.cpp \
      arm/GenPoint.cpp \
      arm/GenScanline.cpp \
      arm/GenTriangle.cpp \
      codegen/arm-codegen.c \
      codegen/arm-codegen.h \
      codegen/arm-dis.c \
      codegen/arm-dis.h \
      codegen/arm_dpimacros.h \
      codegen/bitset.c \
      codegen/bitset.h \
      codegen/codegen.h \
      codegen/emit.c \
      codegen/emit.h \
      codegen/heap.c \
      codegen/heap.h \
      codegen/instruction.c \
      codegen/instruction.h \
      codegen/segment.c \
      codegen/segment.h \
      linux-x11/ContextLinux.cpp \
      linux-x11/Surface.cpp \
      linux-x11/Surface.h \
      linux-x11/e32def.h \
      linux-x11/egl.cpp \
      linux-x11/stdafx.cpp \
      linux-x11/stdafx.h
