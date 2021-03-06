---
layout: default
title: Download
---

{% assign glfwversion = site.changelogs.last.title %}
{% assign releasedate = site.changelogs.last.date | date: "%Y-%m-%d" %}

## Download

The current version is **{{ glfwversion }}**, which was released on
<strong>{% include time.html date=releasedate %}</strong>.
See the [release notes](docs/latest/news.html) for details.

### Source package

{% row %}
{% col 2-3 %}
This package contains the complete source code with CMake build files,
[documentation](docs/latest/), examples and test programs. It
is the recommended download for all platforms and offers the most control.

All development is done on GitHub.  The `master` branch is our integration
branch for the next feature release while the `3.3-stable` branch only adds bug
fixes for patch releases.
{% endcol %}
{% col 1-3 %}
{% button https://github.com/glfw/glfw/releases/download/{{ glfwversion }}/glfw-{{ glfwversion }}.zip %}
Source package
{% endbutton %}
{% button https://github.com/glfw/glfw %}
GitHub repository
{% endbutton %}
{% endcol %}
{% endrow %}

### Windows pre-compiled binaries

{% row %}
{% col 2-3 %}
These packages contain the GLFW header files, [documentation](docs/latest/) and
release mode static libraries, DLLs and import libraries for Visual C++
2010-2019, MinGW-w64 and plain MinGW.

Binaries for Visual C++ 2010 and plain MinGW are only available in the 32-bit
package.
{% endcol %}
{% col 1-3 %}
{% button https://github.com/glfw/glfw/releases/download/{{ glfwversion }}/glfw-{{ glfwversion }}.bin.WIN64.zip %}
64-bit Windows binaries
{% endbutton %}
{% button https://github.com/glfw/glfw/releases/download/{{ glfwversion }}/glfw-{{ glfwversion }}.bin.WIN32.zip %}
32-bit Windows binaries
{% endbutton %}
{% endcol %}
{% endrow %}

### macOS pre-compiled binaries

{% row %}
{% col 2-3 %}
This package contains the GLFW header files, [documentation](docs/latest/) and
release mode static and dynamic libraries for macOS 10.8 and later.
{% endcol %}
{% col 1-3 %}
{% button https://github.com/glfw/glfw/releases/download/{{ glfwversion }}/glfw-{{ glfwversion }}.bin.MACOS.zip %}
64-bit macOS binaries
{% endbutton %}
{% endcol %}
{% endrow %}

### Linux and BSD binaries

Check if your package system provides GLFW {{ glfwversion }} or another version
new enough to be useful to you.

If not, please download and [compile GLFW from
source](docs/latest/compile.html).  A source package is available above, or you
could [clone it from GitHub](https://github.com/glfw/glfw).

