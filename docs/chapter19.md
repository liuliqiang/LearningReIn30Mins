# 还有些什么东西没提到

上边已经描述了构造正则表达式的大量元素，但是还有很多没有提到的东西。下面是一些未提到的元素的列表，包含语法和简单的说明。你可以在网上找到更详细的参考资料来学习它们--当你需要用到它们的时候。如果你安装了MSDN Library,你也可以在里面找到.net下正则表达式详细的文档。这里的介绍很简略，如果你需要更详细的信息，而又没有在电脑上安装MSDN Library,可以查看关于正则表达式语言元素的MSDN在线文档。


表7.尚未详细讨论的语法

<table cellspacing="0">
        <thead>
            <tr>
                <th scope="col">代码/语法</th>

                <th scope="col">说明</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><span class="code">\a</span></td>
                <td><span class="desc">报警字符(打印它的效果是电脑嘀一声)</span></td>

            </tr>
            <tr>
                <td><span class="code">\b</span></td>
                <td><span class="desc">通常是单词分界位置，但如果在字符类里使用代表退格</span></td>
            </tr>
            <tr>
                <td><span class="code">\t</span></td>

                <td><span class="desc">制表符，Tab</span></td>
            </tr>
            <tr>
                <td><span class="code">\r</span></td>
                <td><span class="desc">回车</span></td>
            </tr>
            <tr>

                <td><span class="code">\v</span></td>
                <td><span class="desc">竖向制表符</span></td>
            </tr>
            <tr>
                <td><span class="code">\f</span></td>
                <td><span class="desc">换页符</span></td>
            </tr>

            <tr>
                <td><span class="code">\n</span></td>
                <td><span class="desc">换行符</span></td>
            </tr>
            <tr>
                <td><span class="code">\e</span></td>
                <td><span class="desc">Escape</span></td>

            </tr>
            <tr>
                <td><span class="code">\0nn</span></td>
                <td><span class="desc">ASCII代码中八进制代码为nn的字符</span></td>
            </tr>
            <tr>
                <td><span class="code">\xnn</span></td>

                <td><span class="desc">ASCII代码中十六进制代码为nn的字符</span></td>
            </tr>
            <tr>
                <td><span class="code">\unnnn</span></td>
                <td><span class="desc">Unicode代码中十六进制代码为nnnn的字符</span></td>
            </tr>
            <tr>

                <td><span class="code">\cN</span></td>
                <td><span class="desc">ASCII控制字符。比如\cC代表Ctrl+C</span></td>
            </tr>
            <tr>
                <td><span class="code">\A</span></td>
                <td><span class="desc">字符串开头(类似^，但不受处理多行选项的影响)</span></td>
            </tr>

            <tr>
                <td><span class="code">\Z</span></td>
                <td><span class="desc">字符串结尾或行尾(不受处理多行选项的影响)</span></td>
            </tr>
            <tr>
                <td><span class="code">\z</span></td>
                <td><span class="desc">字符串结尾(类似$，但不受处理多行选项的影响)</span></td>

            </tr>
            <tr>
                <td><span class="code">\G</span></td>
                <td><span class="desc">当前搜索的开头</span></td>
            </tr>
            <tr>
                <td><span class="code">\p{name}</span></td>

                <td><span class="desc">Unicode中命名为name的字符类，例如\p{IsGreek}</span></td>
            </tr>
            <tr>
                <td><span class="code">(?&gt;exp)</span></td>
                <td><span class="desc">贪婪子表达式</span></td>
            </tr>
            <tr>

                <td><span class="code">(?&lt;x&gt;-&lt;y&gt;exp)</span></td>
                <td><span class="desc">平衡组</span></td>
            </tr>
            <tr>
                <td><span class="code">(?im-nsx:exp)</span></td>

                <td><span class="desc">在子表达式exp中改变处理选项</span></td>
            </tr>
            <tr>
                <td><span class="code">(?im-nsx)</span></td>
                <td><span class="desc">为表达式后面的部分改变处理选项</span></td>
            </tr>
            <tr>

                <td><span class="code">(?(exp)yes|no)</span></td>
                <td><span class="desc">把exp当作零宽正向先行断言，如果在这个位置能匹配，使用yes作为此组的表达式；否则使用no</span></td>
            </tr>
            <tr>
                <td><span class="code">(?(exp)yes)</span></td>
                <td><span class="desc">同上，只是使用空表达式作为no</span></td>
            </tr>

            <tr>
                <td><span class="code">(?(name)yes|no)</span></td>
                <td><span class="desc">如果命名为name的组捕获到了内容，使用yes作为表达式；否则使用no</span></td>
            </tr>
            <tr>
                <td><span class="code">(?(name)yes)</span></td>
                <td><span class="desc">同上，只是使用空表达式作为no</span></td>

            </tr>
        </tbody>
    </table>