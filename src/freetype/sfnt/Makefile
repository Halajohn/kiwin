include $(MakDir)/Rules.config.lib

all: depend $(LibKwFreetypeSfntObjFiles) $(LibKwFreetypeSfntObjFiles_g)

clean:
	@$(RM) -f *~ .lib_depend .lib_depend_g $(LibKwFreetypeSfntObjFiles) $(LibKwFreetypeSfntObjFiles_g)

depend: .lib_depend .lib_depend_g

ifeq (.lib_depend,$(wildcard .lib_depend))
include .lib_depend
endif

ifeq (.lib_depend_g,$(wildcard .lib_depend_g))
include .lib_depend_g
endif

include $(MakDir)/Rules.build.lib
