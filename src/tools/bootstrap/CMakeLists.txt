# Generated from bootstrap.pro.

#####################################################################
## Bootstrap Module:
#####################################################################

# special case begin
# The bootstrap library has a few manual tweaks compared to other
# libraries.
add_library(Bootstrap STATIC)
# special case end
qt_extend_target(Bootstrap
    SOURCES
        ../../corelib/codecs/qlatincodec.cpp
        ../../corelib/codecs/qtextcodec.cpp
        ../../corelib/codecs/qutfcodec.cpp
        ../../corelib/global/qendian.cpp
        ../../corelib/global/qglobal.cpp
        ../../corelib/global/qlogging.cpp
        ../../corelib/global/qmalloc.cpp
        ../../corelib/global/qnumeric.cpp
        ../../corelib/global/qoperatingsystemversion.cpp
        ../../corelib/global/qrandom.cpp
        ../../corelib/io/qabstractfileengine.cpp
        ../../corelib/io/qbuffer.cpp
        ../../corelib/io/qdebug.cpp
        ../../corelib/io/qdir.cpp
        ../../corelib/io/qdiriterator.cpp
        ../../corelib/io/qfile.cpp
        ../../corelib/io/qfiledevice.cpp
        ../../corelib/io/qfileinfo.cpp
        ../../corelib/io/qfilesystemengine.cpp
        ../../corelib/io/qfilesystementry.cpp
        ../../corelib/io/qfsfileengine.cpp
        ../../corelib/io/qfsfileengine_iterator.cpp
        ../../corelib/io/qiodevice.cpp
        ../../corelib/io/qipaddress.cpp
        ../../corelib/io/qloggingcategory.cpp
        ../../corelib/io/qloggingregistry.cpp
        ../../corelib/io/qresource.cpp
        ../../corelib/io/qsavefile.cpp
        ../../corelib/io/qstandardpaths.cpp
        ../../corelib/io/qtemporarydir.cpp
        ../../corelib/io/qtemporaryfile.cpp
        ../../corelib/io/qurl.cpp
        ../../corelib/io/qurlidna.cpp
        ../../corelib/io/qurlquery.cpp
        ../../corelib/io/qurlrecode.cpp
        ../../corelib/kernel/qcoreapplication.cpp
        ../../corelib/kernel/qcoreglobaldata.cpp
        ../../corelib/kernel/qmetatype.cpp
        ../../corelib/kernel/qsharedmemory.cpp
        ../../corelib/kernel/qsystemerror.cpp
        ../../corelib/kernel/qsystemsemaphore.cpp
        ../../corelib/kernel/qvariant.cpp
        ../../corelib/plugin/quuid.cpp
        ../../corelib/serialization/qcborcommon.cpp
        ../../corelib/serialization/qcborstreamwriter.cpp
        ../../corelib/serialization/qcborvalue.cpp
        ../../corelib/serialization/qdatastream.cpp
        ../../corelib/serialization/qjsonarray.cpp
        ../../corelib/serialization/qjsoncbor.cpp
        ../../corelib/serialization/qjsondocument.cpp
        ../../corelib/serialization/qjsonobject.cpp
        ../../corelib/serialization/qjsonparser.cpp
        ../../corelib/serialization/qjsonvalue.cpp
        ../../corelib/serialization/qjsonwriter.cpp
        ../../corelib/serialization/qtextstream.cpp
        ../../corelib/serialization/qxmlstream.cpp
        ../../corelib/serialization/qxmlutils.cpp
        ../../corelib/text/qbytearray.cpp
        ../../corelib/text/qbytearraylist.cpp
        ../../corelib/text/qbytearraymatcher.cpp
        ../../corelib/text/qlocale.cpp
        ../../corelib/text/qlocale_tools.cpp
        ../../corelib/text/qregexp.cpp
        ../../corelib/text/qstring.cpp
        ../../corelib/text/qstring_compat.cpp
        ../../corelib/text/qstringbuilder.cpp
        ../../corelib/text/qstringlist.cpp
        ../../corelib/text/qstringview.cpp
        ../../corelib/text/qvsnprintf.cpp
        ../../corelib/time/qcalendar.cpp
        ../../corelib/time/qdatetime.cpp
        ../../corelib/time/qgregoriancalendar.cpp
        ../../corelib/time/qromancalendar.cpp
        ../../corelib/tools/qarraydata.cpp
        ../../corelib/tools/qbitarray.cpp
        ../../corelib/tools/qcommandlineoption.cpp
        ../../corelib/tools/qcommandlineparser.cpp
        ../../corelib/tools/qcryptographichash.cpp
        ../../corelib/tools/qhash.cpp
        ../../corelib/tools/qline.cpp
        ../../corelib/tools/qmap.cpp
        ../../corelib/tools/qpoint.cpp
        ../../corelib/tools/qrect.cpp
        ../../corelib/tools/qringbuffer.cpp
        ../../corelib/tools/qsize.cpp
        ../../corelib/tools/qversionnumber.cpp
        ../../xml/dom/qdom.cpp
        ../../xml/sax/qxml.cpp
    PUBLIC_DEFINES # special case
        QT_VERSION_MAJOR=${PROJECT_VERSION_MAJOR} # special case
        QT_VERSION_MINOR=${PROJECT_VERSION_MINOR} # special case
        QT_VERSION_PATCH=${PROJECT_VERSION_PATCH} # special case
        QT_VERSION_STR="${PROJECT_VERSION}" # special case
        QT_USE_QSTRINGBUILDER # special case
        QT_BOOTSTRAPPED
        QT_NO_CAST_FROM_ASCII
        QT_NO_CAST_TO_ASCII
        QT_NO_FOREACH
    INCLUDE_DIRECTORIES
        ..
        ../../3rdparty/tinycbor/src
    PUBLIC_INCLUDE_DIRECTORIES  # special case
        $<TARGET_PROPERTY:Core,INCLUDE_DIRECTORIES> # special case
        $<TARGET_PROPERTY:Xml,INCLUDE_DIRECTORIES> # special case
    PUBLIC_LIBRARIES  # special case
        Qt::Platform # special case
)

#### Keys ignored in scope 1:.:.:bootstrap.pro:<TRUE>:
# INSTALLS = "lib"
# MODULE_CONFIG = "gc_binaries"
# MODULE_INCNAME = "QtCore" "QtXml"
# _OPTION = "host_build"
# lib.CONFIG = "dummy_install"

## Scopes:
#####################################################################

qt_extend_target(Bootstrap CONDITION UNIX
    SOURCES
        ../../corelib/io/qfilesystemengine_unix.cpp
        ../../corelib/io/qfilesystemiterator_unix.cpp
        ../../corelib/io/qfsfileengine_unix.cpp
        ../../corelib/kernel/qcore_unix.cpp
        ../../corelib/kernel/qsharedmemory_posix.cpp
        ../../corelib/kernel/qsharedmemory_systemv.cpp
        ../../corelib/kernel/qsharedmemory_unix.cpp
        ../../corelib/kernel/qsystemsemaphore_posix.cpp
        ../../corelib/kernel/qsystemsemaphore_systemv.cpp
        ../../corelib/kernel/qsystemsemaphore_unix.cpp
)

qt_extend_target(Bootstrap CONDITION WIN32
    SOURCES
        ../../corelib/global/qoperatingsystemversion_win.cpp
        ../../corelib/io/qfilesystemengine_win.cpp
        ../../corelib/io/qfilesystemiterator_win.cpp
        ../../corelib/io/qfsfileengine_win.cpp
        ../../corelib/io/qstandardpaths_win.cpp
        ../../corelib/kernel/qcoreapplication_win.cpp
        ../../corelib/kernel/qsharedmemory_win.cpp
        ../../corelib/kernel/qsystemsemaphore_win.cpp
        ../../corelib/kernel/qwinregistry.cpp
        ../../corelib/plugin/qsystemlibrary.cpp
    PUBLIC_LIBRARIES
        advapi32
        netapi32
        ole32
        shell32
        user32
)

qt_extend_target(Bootstrap CONDITION APPLE
    SOURCES
        ../../corelib/global/qoperatingsystemversion_darwin.mm
        ../../corelib/kernel/qcore_foundation.mm
        ../../corelib/kernel/qcore_mac.cpp
        ../../corelib/kernel/qcore_mac_objc.mm
        ../../corelib/kernel/qcoreapplication_mac.cpp
    PUBLIC_LIBRARIES
        ${FWFoundation}
)

qt_extend_target(Bootstrap CONDITION APPLE_OSX
    SOURCES
        ../../corelib/io/qstandardpaths_mac.mm
    LIBRARIES
        ${FWCoreServices}
)

qt_extend_target(Bootstrap CONDITION APPLE_UIKIT
    LIBRARIES
        ${FWUIKit}
)

qt_extend_target(Bootstrap CONDITION UNIX AND NOT APPLE_OSX
    SOURCES
        ../../corelib/io/qstandardpaths_unix.cpp
)

qt_extend_target(Bootstrap CONDITION CMAKE_CROSSCOMPILING OR NOT QT_FEATURE_system_zlib
    SOURCES
        ../../3rdparty/zlib/src/adler32.c
        ../../3rdparty/zlib/src/compress.c
        ../../3rdparty/zlib/src/crc32.c
        ../../3rdparty/zlib/src/deflate.c
        ../../3rdparty/zlib/src/gzclose.c
        ../../3rdparty/zlib/src/gzlib.c
        ../../3rdparty/zlib/src/gzread.c
        ../../3rdparty/zlib/src/gzwrite.c
        ../../3rdparty/zlib/src/infback.c
        ../../3rdparty/zlib/src/inffast.c
        ../../3rdparty/zlib/src/inflate.c
        ../../3rdparty/zlib/src/inftrees.c
        ../../3rdparty/zlib/src/trees.c
        ../../3rdparty/zlib/src/uncompr.c
        ../../3rdparty/zlib/src/zutil.c
    INCLUDE_DIRECTORIES
        ../../3rdparty/zlib/src
)

qt_extend_target(Bootstrap CONDITION QT_FEATURE_system_zlib AND NOT CMAKE_CROSSCOMPILING
    LIBRARIES
        ZLIB::ZLIB
)

qt_extend_target(Bootstrap CONDITION WIN32 AND mingw
    PUBLIC_LIBRARIES
        uuid
)

# special case begin
qt_internal_add_link_flags_gc_sections(Bootstrap PUBLIC)
set_target_properties(Bootstrap PROPERTIES AUTOMOC OFF AUTOUIC OFF AUTORCC OFF)
qt_internal_add_target_aliases(Bootstrap)
qt_enable_msvc_cplusplus_define(Bootstrap PUBLIC)
# special case end
