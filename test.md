# Best Practice Name

|  |  |
| --- | --- |
| Target audience | (e.g. UI developers / BE developers / QA…) |
| Associated technology | (language, framework) |
| Prerequisites | (e.g. being familiar with React) |

## tl;dr

Short summary of the recommended best practices

## Introduction

Explain the best practice topic.

## Training

List of available training, courses that portray to the topic.

## Best Practices

### Practice 1

Description

**Example**

<table>
  <tr>
    <td>
        <strong>Good</strong>
    </td>
    <td>
        <strong>Bad</strong>
    </td>
  </tr>
  <tr>
    <td>
       <pre>
        <code class="language-javascript">

const Headline = styled.h1\`
    color: ${(p) => p.color}; // short variable
\`;

const Text = styled.span\`
    padding: ${({ padding }) => padding}px; // Or destructure
\`;
            </code>
        </pre>
    </td>
    <td>
        <pre>
            <code class="language-javascript">

const Headline = styled.h1\`
    color: ${(componentProperties) => componentProperties.color};  // Too long variable
\`;
            </code>
        </pre>
    </td>
    <td>
        <pre>
            <code class="language-javascript">
const Headline = styled.h1\`
    color: ${(componentProperties) => componentProperties.color};  // Too long variable
\`;
            </code>
        </pre>
    </td>
  </tr>
</table>


Special conditions

Reference
