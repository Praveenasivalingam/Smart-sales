from flask import Flask, render_template, request
import webview
import threading

app = Flask(__name__)

# -----------------------------
# Home Page
# -----------------------------
@app.route("/", methods=["GET", "POST"])
def index():

    error = None
    summary_table = None
    plot1 = None
    plot2 = None

    if request.method == "POST":

        uploaded_file = request.files.get("file")

        if uploaded_file is None or uploaded_file.filename == "":
            error = "Please upload a CSV or Excel file."

        else:
            # Demo output
            summary_table = """
            <table class="table table-striped table-hover">
                <thead>
                    <tr>
                        <th>Date</th>
                        <th>Predicted Sales</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>2026-08-01</td>
                        <td>₹45,000</td>
                    </tr>
                    <tr>
                        <td>2026-08-15</td>
                        <td>₹52,000</td>
                    </tr>
                    <tr>
                        <td>2026-09-01</td>
                        <td>₹60,000</td>
                    </tr>
                </tbody>
            </table>
            """

    return render_template(
        "index.html",
        error=error,
        summary_table=summary_table,
        plot1=plot1,
        plot2=plot2
    )


# -----------------------------
# Start Flask Server
# -----------------------------
def start_flask():
    app.run(
        host="127.0.0.1",
        port=5000,
        debug=False,
        use_reloader=False
    )


# -----------------------------
# Android-Style Frame
# -----------------------------
if __name__ == "__main__":

    flask_thread = threading.Thread(
        target=start_flask,
        daemon=True
    )

    flask_thread.start()

    webview.create_window(
        "Sales Forecaster",
        "http://127.0.0.1:5000",
        width=400,
        height=800,
        resizable=True
    )

    webview.start()
