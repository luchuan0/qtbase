# Generated from minimal.pro.

#####################################################################
## QMinimalIntegrationPlugin Plugin:
#####################################################################

qt_find_package(WrapFreetype PROVIDED_TARGETS WrapFreetype::WrapFreetype) # special case

qt_add_plugin(QMinimalIntegrationPlugin
    OUTPUT_NAME qminimal
    TYPE platforms
    DEFAULT_IF ${QT_QPA_DEFAULT_PLATFORM} MATCHES minimal # special case
    SOURCES
        main.cpp
        qminimalbackingstore.cpp qminimalbackingstore.h
        qminimalintegration.cpp qminimalintegration.h
    DEFINES
        QT_NO_FOREACH
    PUBLIC_LIBRARIES
        Qt::Core
        Qt::CorePrivate
        Qt::EventDispatcherSupportPrivate
        Qt::FontDatabaseSupportPrivate
        Qt::Gui
        Qt::GuiPrivate
)

#### Keys ignored in scope 1:.:.:minimal.pro:<TRUE>:
# OTHER_FILES = "minimal.json"

## Scopes:
#####################################################################

qt_extend_target(QMinimalIntegrationPlugin CONDITION QT_FEATURE_freetype
    LIBRARIES
        WrapFreetype::WrapFreetype
)

#### Keys ignored in scope 3:.:.:minimal.pro:NOT TARGET___equals____ss_QT_DEFAULT_QPA_PLUGIN:
# PLUGIN_EXTENDS = "-"
