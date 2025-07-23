# Resolving the “OLE Automation Error”

If you see this message:

**“Microsoft Excel is waiting for another application to complete an OLE action.”**

<div align="left"><figure><img src="../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure></div>

It means Excel tried to communicate with another program (like a browser or script), but got stuck. This often happens during automation.

**How to fix it**

1. Go to **File** → **Options** → **Advanced**
2. Scroll to the **General** section
3. Uncheck **Ignore other applications that use Dynamic Data Exchange (DDE)**
4. Click **OK**
5. Close Excel and **restart your computer**

That should solve it.
