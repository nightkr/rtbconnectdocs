Authentication is requested by the server when the client connects. Usually a request conversation looks like this:

    >> <auth type="get" />
    << <auth type="set" id="(REQUEST_ID)"><id>(BL_ID)</id><username>(BL_NAME)</username></auth>

This can trigger one of two responses.

If it succeeds it looks like this:

    >> <auth type="result"><success /></auth>

Otherwise it looks like this:

    >> <auth type="result"><fail>(MESSAGE)</fail></auth>

or this:

    >> <auth type="result"><fail /></auth>
