# js-selfhosting
Javascript based URL abuse selfhosting. This requires only one 'everything.html' file and the rest of the webpage is hosted in the URL, on the client machine. Credits: xqt2.com
The everything.html file includes a client-side loader to read, decompress and evaluate the URL.

To make your own page, visit <a href="http://shubhamgg.github.io/js-selfhosting">shubhamgg.github.io/js-selfhosting</a>
Then using your browsers web-dev tools (inspect element), edit the code of the page to make your own page (you might want to keep the little script in body that sets the title). After that, call <code>make()</code> in the console to generate your own page.

For more details, visit:
http://xqt2.com/p/everything.html#DwIw9gJgngBAzgFygGwKYF4BEAHAhhCASwDsBzALhgEZUBbAbhltwA8BaAd0IgQAtKALAAY6jZgCdSJNmgBmCSrgCuCMGNyTp4wqV4KYy1fUwA+AFAwYwXlXhI0WBKhYI2uZDuKUAxqmJPxYxMAQRAlOBJSGD5UGABVACUAGQBCYAB6G3NLYGwQ5GQYDl5cBBgoMCV4VFjeVHFYwjgYbzB-PzLW-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-K+P0-5U6NWZMltT4QgNJ7NVaRy1UqGKgKAJqcQI2FgI2AidIdUHmd1GuVke4hAT4WZu4naEO6qhAKGAEHaNiUgKGWqRaU-VAfK4ISWHWxg+GW0qzUU7AEAcOYII+Hh3SPZvdOeo2CybFT4XAWQRYSaWyMlJyz4AecMitBoXRKAA5DgXSKYyacQAyRaa0ZfPFXkg2bwDTfHcaHaVJeGO3H8jGfN-N9IIQOk3ACMcmeBqGWgdUEFHmCGgQdJnk8zO-YIDgVFyXMATRTO+6TMymJQJxFqKsVaNiAw7wGscQ1pAym5U6fSuIJqEAeGtWU6ZalmB2jsCAXSLNFqO6R5GM8ROOfUxJeI1BYIWQAyKe-cVUvGZgazL8H0z-d9pqUqRaKJFAtWKB2gIhUaWQVAUtT9KxOIaXew8acsd7R8tWOIBjBbJISTaHEFHqIQbwZFFE3NWQFR7AVaMynOGGZAFqQVPlVZEUp5AO64GM1AYIPRgcpQFgTXNxli14x0s-NiDXFqXfBAcQUsAQP6vQ3AaE-10sQxNmSTe9l6U+KxN8akVc9QpUvBdPCGT4SaU6XnN8dGRZWQXgFo8UvpotBK2RtRYgP4oEsCeGOV+6XgcaHsR+JICMdUWQZt7hRYGwWgU6HaOAUsSjCTTA1adUCIk9KZJIKqbqPfUqUTIms5giAiVaX60tmTnfCpbcBKwcz4LgFaPZIgj4-dnxsLGGGGAydIZ60gM7bdmykRZg3pKzKsFqFgQgdufGgLosyhWdCfI2cMqFtHcT64EAFwGGVHYIdUYaOIb2Ty06KrL7giW+dUEGCGF6IQpIAiGFc9XScqGsFHa2kASZ4IYkpIcQGdXNTqIz2qGacaKsbAdbPYhIRhWgegqZKJhIKyzrF6AidpUseHcaMuh4N2flpp4VT7xTBPHZFgCGHaGL2VHb4UtOsAOjBAXSL-RuVAKsCGdUO0io7RJap+w4L8KAaR+lRYMpWqRdFQ8aagmxPSytlgKgHqQJUsJIVaJqCTJQF9IPYgfLYgOFaDL8F6Zqo-cQb7VaNWdUaZ80sAU6T4FT1TbDQgNbOeNr4XbwHqEAIau7SaVaSUuANzdBr2BAS2FgT+KGRaJWsE3-HaR-Q4iY9r1o8EgyGGOAFmwlxaQyH-RVUqR+4Q0aK1iMI2G+neb3ilBABstxhHet8sR5wgfexWlo52JIXScYtpLcMsljOIKGKVDhSacIYW4UqGGyWAtie6WQLem4U6csa4MCpFUnLP2yp6l9RLTO15Qs3OJqcsT+aqguZAGxKis3NiZt8VFPLbKNbwTLRYus9IcaLKF-LQCNhAYdovABIEDFro9RZAPpEALvyhgQAAyslJQPRygD6QIAIAAyEIAEClQxe3HZVJLCSBuwREyqfRGelLDPE4SCWMACtCoDiAda0VXSOcnSCGlkkuRY2kkEWaAhSoEANiKkWy55UlAtOBqjWFoTi40YcScBLQGrpBxdINYAiGvHtJmd7KhAM5gvWcBQBaA3gK4JomhwsVdcicNWM83pxoZnUGeIanklMSfAIwrnJQEoFqIZkke1wAyFDCqinRdI3gKqEoH3iLRVoBkcCLICIQc8IiasUmkIGMx9RfB2WFCtSj7ykoNe4yfePdjPSIJa6I+VJKbGLR6EDo3cYRJjgvSrYEgscQhIgWwB-lJoHAfFK7j-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
