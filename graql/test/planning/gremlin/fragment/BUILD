#
# Copyright (C) 2020 Grakn Labs
#
# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU Affero General Public License as
# published by the Free Software Foundation, either version 3 of the
# License, or (at your option) any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU Affero General Public License for more details.
#
# You should have received a copy of the GNU Affero General Public License
# along with this program.  If not, see <https://www.gnu.org/licenses/>.
#

load("@graknlabs_dependencies//tool/checkstyle:rules.bzl", "checkstyle_test")

java_test(
    name = "in-plays-fragment-test",
    size = "small",
    srcs = ["InPlaysFragmentTest.java"],
    test_class = "grakn.core.graql.planning.gremlin.fragment.InPlaysFragmentTest",
    deps = [
        "//core",
        "@maven//:com_google_guava_guava",
        "@maven//:org_apache_tinkerpop_gremlin_core",
        "//graql/planning",
        "@graknlabs_graql//java:graql",
    ],
)

java_test(
    name = "isa-explicit-test",
    size = "small",
    srcs = ["IsaExplicitTest.java"],
    test_class = "grakn.core.graql.planning.gremlin.fragment.IsaExplicitTest",
    deps = ["@graknlabs_graql//java:graql"],
)

java_test(
    name = "out-plays-fragment-test",
    size = "small",
    srcs = ["OutPlaysFragmentTest.java"],
    test_class = "grakn.core.graql.planning.gremlin.fragment.OutPlaysFragmentTest",
    deps = [
        "//core",
        "@maven//:com_google_guava_guava",
        "@maven//:org_apache_tinkerpop_gremlin_core",

        "//graql/planning",
        "@graknlabs_graql//java:graql",
    ],
)

checkstyle_test(
    name = "checkstyle",
    targets = [
        ":in-plays-fragment-test",
        ":isa-explicit-test",
        ":out-plays-fragment-test",
    ],
)
