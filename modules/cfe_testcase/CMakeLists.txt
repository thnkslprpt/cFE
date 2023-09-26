include_directories(inc)

# Filenames based on doxygen groups.
# Create the app module
add_cfe_app(cfe_testcase
    src/cfe_test.c
)

# register the dependency on cfe_assert
add_cfe_app_dependency(cfe_testcase cfe_assert)
add_cfe_tables(cfeTestAppTable tables/cfe_test_tbl.c)
