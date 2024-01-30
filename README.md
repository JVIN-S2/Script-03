iface = qgis.utils.iface
source = QgsProject.instance().mapLayersByName(the name of the layer: jv insfran)[0]
iface.setActiveLayer( source )
iface.actionCopyFeatures().trigger()
target = QgsProject.instance().mapLayersByName(the name of the layer: jv insfran)[0]
iface.setActiveLayer( target )
iface.actionPasteFeatures().trigger()
target.removeSelection()
iface.setActiveLayer( source )
