Finagle backend
===============

To use, add the following dependency to your project::

  "com.softwaremill.sttp.client" %% "finagle-backend" % "2.0.0-RC5"

This backend depends on `finagle <https://twitter.github.io/finagle/>`_, and offers an asynchronous backend, which
wraps results in Twitter's ``Future``.

Please note that:
* the backend does not support ``SttpBackendOptions``, that is specifying proxy settings (proxies are not implemented
in http4s, see `this issue <https://github.com/http4s/http4s/issues/251>`_), as well as configuring the connect timeout
* the backend does not support streaming or websockets
