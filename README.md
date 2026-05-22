from flask import Flask, render_template_string

app = Flask(__name__)

products = [
    {
        "name": "Shoes",
        "price": "₹1999",
        "image": "https://images.unsplash.com/photo-1542291026-7eec264c27ff"
    },
    {
        "name": "Watch",
        "price": "₹2999",
        "image": "https://images.unsplash.com/photo-1523275335684-37898b6baf30"
    },
    {
        "name": "T-Shirt",
        "price": "₹999",
        "image": "https://images.unsplash.com/photo-1521572163474-6864f9cf17ab"
    },
    {
        "name": "Headphones",
        "price": "₹1499",
        "image": "https://images.unsplash.com/photo-1505740420928-5e560c06d30e"
    }
]

HTML = """
<!DOCTYPE html>
<html>
<head>
    <title>Shopping App</title>

    <style>
        body{
            margin:0;
            font-family:Arial;
            background:#111;
            color:white;
        }

        .navbar
